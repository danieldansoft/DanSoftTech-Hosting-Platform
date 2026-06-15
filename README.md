# DanSoftTech-Hosting-Platform

Infrastructure Lab based on Windows Server 2025, Cloudflare Tunnel, Apache/XAMPP, Active Directory, OpenSSH/SFTP, and multi-site hosting.

## Provisionamento de Subdomínios no Windows Server 2025

Documentação operacional para criação e publicação de novos subdomínios utilizando:

* Windows Server 2025
* Apache (XAMPP)
* Cloudflare Tunnel
* OpenSSH/SFTP
* Active Directory
* FileZilla
* MikroTik RouterOS

## Ambiente

### Infraestrutura Física

- SERVER2025
- NVMe Kingston 1TB
- 16GB RAM
- Nobreak PW 2000
- Ambiente climatizado
- Estação Ryzen 5 5600GT com 32GB RAM

### Servidor
- Windows Server 2025
- NVMe SSD 1TB
- 16GB RAM
- Apache/XAMPP
- Cloudflare Tunnel
- OpenSSH Server
- Active Directory

### Estação de Gerenciamento
- AMD Ryzen 5 5600GT
- 32GB RAM
- FileZilla
- Visual Studio Code

## Arquitetura

```text
Internet
   ↓
Cloudflare Tunnel
   ↓
Apache/XAMPP
   ↓
VirtualHosts
   ↓
HTDOCS
   ↓
SFTP Chroot
```

---

## 1. Criar rota DNS no Cloudflare Tunnel

Exemplo:

```powershell
cloudflared tunnel route dns dansoftech suporte.dansoftech.com.br

taskkill /F /IM cloudflared.exe

Start-Service Cloudflared

sc query Cloudflared
```

---

## 2. Criar pasta do site

CMD:

```cmd
cmd /c mkdir C:\xampp\htdocs\suporte
```

PowerShell:

```powershell
mkdir C:\xampp\htdocs\suporte
```

---

## 3. Adicionar no config.yml

Adicionar na penúltima linha:

```yaml
- hostname: suporte.dansoftech.com.br
  service: http://127.0.0.1:80
```

---

## 4. Backup do VirtualHost

```powershell
if (!(Test-Path "C:\Backup")) {
    New-Item -ItemType Directory -Path "C:\Backup"
}

$Data = Get-Date -Format "yyyy-MM-dd_HH-mm"

Copy-Item `
"C:\xampp\apache\conf\extra\httpd-vhosts.conf" `
"C:\Backup\httpd-vhosts_$Data.bak"
```

---

## 5. Adicionar VirtualHost

```apache
<VirtualHost *:80>
    ServerName suporte.dansoftech.com.br

    DocumentRoot "C:/xampp/htdocs/suporte"

    <Directory "C:/xampp/htdocs/suporte">
        AllowOverride All
        Require all granted
        Options -Indexes
    </Directory>

    ErrorLog "logs/suporte_error.log"
    CustomLog "logs/suporte_access.log" combined
</VirtualHost>
```

---

## 6. Validar e reiniciar Apache

```powershell
Stop-Service Apache2.4 -Force -ErrorAction SilentlyContinue

C:\xampp\apache\bin\httpd.exe -t
# Resultado esperado:
# Syntax OK

Restart-Service Apache2.4 -Force -ErrorAction SilentlyContinue

Get-Service Apache2.4
```

---

## 7. Reiniciar Cloudflare

```powershell
taskkill /F /IM cloudflared.exe

Start-Service Cloudflared

sc query Cloudflared

Get-Service Cloudflared
```

---

## 8. Validar DNS

```powershell
nslookup suporte.dansoftech.com.br
```

ou

```powershell
Resolve-DnsName suporte.dansoftech.com.br
```

---

## 9. Criar Symlink SFTP

```cmd
cmd /c mklink /D C:\SFTP\htdocs\suporte C:\xampp\htdocs\suporte
```

Validar:

```powershell
dir C:\SFTP\htdocs

# ou

Test-Path C:\SFTP\htdocs\suporte
```

---

## Checklist Final

* [x] DNS Cloudflare criado
* [x] Pasta HTDOCS criada
* [x] config.yml atualizado
* [x] Backup realizado
* [x] VirtualHost criado
* [x] Apache validado (Syntax OK)
* [x] Apache reiniciado
* [x] Cloudflared reiniciado
* [x] Symlink SFTP criado
* [x] Teste HTTP OK
* [x] Teste SFTP OK

## Subdomínios Ativos

- https://dansoftech.com.br
- https://suporte.dansoftech.com.br
- https://cris.dansoftech.com.br
- https://tecnetsys.dansoftech.com.br
- https://formulario.dansoftech.com.br

## Status Final

🟢 SUBDOMÍNIO ONLINE E FUNCIONAL

---

**Autor:** Daniel Cerri Ribeiro
**Projeto:** DanSoftTech Infrastructure Lab
