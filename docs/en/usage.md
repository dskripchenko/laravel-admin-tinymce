---
title: Usage
locale: en
status: stable
---

# Usage

```php
Wysiwyg::make('body')->plugins(['advcode', 'autoresize']);
```

For self-hosted TinyMCE, copy the package files to public:

```bash
php artisan vendor:publish --tag=tinymce-assets
```

Then point TinyMCE to the local path:

```js
window.tinyMCE.init({ ..., 'script_src': '/vendor/tinymce/tinymce.min.js' })
```

