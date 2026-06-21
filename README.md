# cf7-add-password-field

The plugin is to add a password filed to Contact form 7 plugin.


Please see https://wordpress.org/plugins/cf7-add-password-field/ .

## Font Awesome stylesheet

This plugin loads the bundled Font Awesome stylesheet by default.

If your theme or another plugin already loads Font Awesome 6, you can dequeue this plugin's stylesheet.

If you want to use another Font Awesome source, such as a CDN, dequeue the bundled stylesheet and enqueue your own stylesheet from your theme or custom plugin.

```php
add_action( 'wp_enqueue_scripts', function() {
    wp_dequeue_style( 'cf7_add_password_field_style' );

    wp_enqueue_style(
        'my-font-awesome',
        'https://example.com/path/to/font-awesome.css',
        array(),
        null
    );
}, 20 );
```

Replace the example URL with the URL of your preferred Font Awesome stylesheet.

Loading stylesheets from third-party services may have privacy, availability, and security implications.
