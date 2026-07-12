<h1 align="center">
  <img src="icon.png" alt="Icon"/>
</h1>

# Blade Google Material Symbols

A package to easily make use of Google's Material Symbols in your Laravel Blade views.  
For a full list of available icons you can preview them at [Material Symbols](https://fonts.google.com/icons?icon.set=Material+Symbols).

To keep the package size manageable, the icons (160,000+) are split into separate repositories by weight.

## Packages
| Weight | Repository                                                                                              | Composer Package                                |
|--------|---------------------------------------------------------------------------------------------------------|-------------------------------------------------|
| 100    | [blade-google-material-symbols-100](https://github.com/richardDobron/blade-google-material-symbols-100) | richarddobron/blade-google-material-symbols-100 |
| 200    | [blade-google-material-symbols-200](https://github.com/richardDobron/blade-google-material-symbols-200) | richarddobron/blade-google-material-symbols-200 |
| 300    | [blade-google-material-symbols-300](https://github.com/richardDobron/blade-google-material-symbols-300) | richarddobron/blade-google-material-symbols-300 |
| 400    | [blade-google-material-symbols-400](https://github.com/richardDobron/blade-google-material-symbols-400) | richarddobron/blade-google-material-symbols-400 |
| 500    | [blade-google-material-symbols-500](https://github.com/richardDobron/blade-google-material-symbols-500) | richarddobron/blade-google-material-symbols-500 |
| 600    | [blade-google-material-symbols-600](https://github.com/richardDobron/blade-google-material-symbols-600) | richarddobron/blade-google-material-symbols-600 |
| 700    | [blade-google-material-symbols-700](https://github.com/richardDobron/blade-google-material-symbols-700) | richarddobron/blade-google-material-symbols-700 |

## Requirements

- PHP 7.4 or higher
- Laravel 8.0 or higher

## Installation

As Material Symbols offers a lot of different styles, you can choose a specific one by using the corresponding package.  

## Usage

Icons can be used as self-closing Blade components which will be compiled to SVG icons:

```blade
<x-gms:500-fact_check-fill-outlined/>
```

You can also pass classes to your icon components:

```blade
<x-gms:600-fact_check-outlined class="w-6 h-6 text-gray-500"/>
```

And even use inline styles:

```blade
<x-gms:700-fact_check-fill-rounded style="color: #555"/>
```

## Configuration

Blade Material Symbols also offers the ability to use features from Blade Icons like default classes, default attributes, etc. If you'd like to configure these, publish the `blade-gms.php` config file:

```bash
php artisan vendor:publish --tag=blade-material-symbols-600-config
```

## Blade Icons

Blade Material Symbols uses Blade Icons under the hood. Please refer to [the Blade Icons readme](https://github.com/driesvints/blade-icons) for additional functionality. We also recommend to [enable icon caching](https://github.com/driesvints/blade-icons#caching) with this library.

Then use them in your views like:

```blade
<img src="{{ asset('vendor/blade-material-symbols-600/star-fill-outlined.svg') }}" width="10" height="10"/>
```

## Maintainers

Blade Material Symbols is developed and maintained by Richard Dobroň.

## License

Blade Material Symbols is open-sourced software licensed under [the MIT license](LICENSE.md).