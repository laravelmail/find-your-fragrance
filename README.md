# Find Your Fragrance

This email template is a marketing message aimed at promoting fragrances in the Fashion & Cosmetics industry. It invites recipients to discover their perfect scent.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Fashion & Cosmetics
- **Message Type:** Marketing
- **Tags:** discovery, perfume, fragrance, cologne

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/find-your-fragrance.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/find-your-fragrance/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.find-your-fragrance',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
