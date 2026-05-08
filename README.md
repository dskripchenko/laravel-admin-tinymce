# dskripchenko/laravel-admin-tinymce

> 🌐 **English** · [Русский](README.ru.md) · [Deutsch](README.de.md) · [中文](README.zh.md)

Alternative WYSIWYG engine on top of TinyMCE. Bring your own license key (TinyMCE is GPL/commercial).

A sister-pack for [`dskripchenko/laravel-admin`](https://github.com/dskripchenko/laravel-admin).

[![Packagist](https://img.shields.io/packagist/v/dskripchenko/laravel-admin-tinymce)](https://packagist.org/packages/dskripchenko/laravel-admin-tinymce)
[![License](https://img.shields.io/packagist/l/dskripchenko/laravel-admin-tinymce)](LICENSE)

## Install

```bash
composer require dskripchenko/laravel-admin-tinymce
php artisan migrate
```

The plugin auto-registers via Laravel package discovery. To publish the
config:

```bash
php artisan vendor:publish --tag=tinymce-config
```

## Documentation

- [Getting started](docs/en/getting-started.md)
- [Usage](docs/en/usage.md)

## License

[MIT](LICENSE) © Denis Skripchenko
