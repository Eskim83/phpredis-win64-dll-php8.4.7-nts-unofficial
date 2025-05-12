# phpredis-win64-dll-php8.4.7-nts-unofficial

This repository contains an **unofficial precompiled DLL** of the [phpredis](https://github.com/phpredis/phpredis) extension for **PHP 8.4.7 NTS** on Windows.

## 🛠 Build Details

* **Extension:** phpredis
* **Version:** 6.2.0
* **PHP Version:** 8.4.7
* **Thread Safety:** **Non-Thread Safe (NTS)**
* **Architecture:** x64 (Windows 64-bit)
* **Compiler:** Visual Studio 2022 (VC17)
* **Build Date:** 2025-05-09

## 📦 Usage

1. Copy `php_redis.dll` to your PHP `ext/` directory (e.g. `C:/laragon/bin/php/php-8.4.7-nts-Win32-vs17-x64/ext/`).
2. Edit your `php.ini` and add the following line **anywhere near other `extension=` entries**:

```ini
extension=php_redis.dll
```

3. Restart your web server or PHP runtime (e.g. Laragon or terminal).
4. Verify installation using:

```bash
php -m
```

or

```bash
php -i | findstr redis
```

## 📌 Notes

* This DLL was compiled manually using the official PHP SDK for Windows.
* It is **not** an official release. Use at your own risk.
* Only compatible with **PHP 8.4.7 NTS x64 VC17** builds.
* Not compatible with TS versions of PHP.

## 📖 Related Article

See full step-by-step guide (in Polish):
👉 [https://eskim.pl/jak-skompilowac-php\_redis-dll-dla-php-8-4-x-na-windowsie-laragon-vs17-ts-nts/](https://eskim.pl/jak-skompilowac-php_redis-dll-dla-php-8-4-x-na-windowsie-laragon-vs17-ts-nts/)

## 📄 License

This DLL was built from the original [phpredis source](https://github.com/phpredis/phpredis), which is released under the [BSD-3-Clause License](https://opensource.org/licenses/BSD-3-Clause).

> All rights belong to the original authors.

---

## ☕ Support

If this saved you time or frustration, feel free to buy me a coffee:
[https://www.buymeacoffee.com/eskim](https://www.buymeacoffee.com/eskim)
