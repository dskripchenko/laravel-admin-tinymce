---
title: Getting Started
locale: en
status: stable
---

# Getting Started

`dskripchenko/laravel-admin-tinymce` is a sister-pack of `dskripchenko/laravel-admin`.
Install once — it auto-registers and surfaces in your admin.

## Install

```bash
composer require dskripchenko/laravel-admin-tinymce
php artisan migrate
```

## Configure

```bash
php artisan vendor:publish --tag=tinymce-config
```

Edit `config/tinymce.php`.


## What it adds

`@dskripchenko/laravel-admin-tinymce` registers a `TinyMceField` for
the `Wysiwyg` slot.

```js
import { TinyMceField } from '@dskripchenko/laravel-admin-tinymce'
import { registerField } from '@dskripchenko/laravel-admin'

registerField('wysiwyg', TinyMceField)
```

You provide a TinyMCE license key (TinyMCE Cloud or self-hosted).

```php
// config/admin-tinymce.php
'api_key' => env('TINYMCE_API_KEY'),
'plugins' => 'lists link image code table',
'toolbar' => 'undo redo | bold italic | link image | code',
```

## See also

- [Usage](usage.md)
- [Glossary](https://github.com/dskripchenko/laravel-admin/blob/main/docs/en/glossary.md)
