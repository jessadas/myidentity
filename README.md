# myidentity
# MyIdentity

ระบบเปลี่ยนรหัสผ่าน AD, Forgot OTP, Unlock Account พร้อมตรวจ LDAPS Certificate

## Requirements
- PHP 8.4
- XAMPP หรือ PHP + Apache
- MySQL
- Windows Server AD with LDAPS

## Installation
1. Clone หรือ Download ZIP
2. แตกไฟล์ไปไว้ใน `htdocs/myidentity`
3. สร้างฐานข้อมูล MySQL แล้วรัน `install.sql`
4. แก้ config ใน:
   - `includes/ldap/ldap_config.php`
   - `cert_checker/read_cert_info.php`
5. รัน `check_ldaps_cert.ps1` ใน Powershell
6. เปิดใช้งานผ่านเว็บเบราว์เซอร์เช่น `http://localhost/myidentity/`

## Features
- Change password via LDAPS
- Forgot Password (OTP)
- Unlock account
- Admin Panel
- Certificate checker & exporter
