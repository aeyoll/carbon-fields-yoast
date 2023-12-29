# Carbon Fields Yoast

__Carbon Fields Yoast__ is an addon to Carbon Fields that allows developers to choose which fields from Carbon Fields to include in the Yoast readability score meter.

## How to use?

Install via composer, in your theme repository:

```bash
composer require aeyoll/carbon-fields-yoast
```

In `functions.php`, add the following:

```php
add_action( 'after_setup_theme', 'crb_initialize_carbon_yoast' );
function crb_initialize_carbon_yoast() {
	include_once __DIR__ . '/vendor/autoload.php';

	new \Carbon_Fields_Yoast\Carbon_Fields_Yoast;
}
```
