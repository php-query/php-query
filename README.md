# phpQuery

phpQuery is a PHP library that enables you to parse HTML and manipulate the DOM using jQuery-like syntax. This repository aims to create a PHP 8.x ready version derived from the original code available in the [Google Code Archive](https://code.google.com/archive/p/phpquery/).

## License

This project is based on the original code released under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contribution Guidelines

We welcome and appreciate contributions from the community. If you'd like to contribute, please follow these guidelines:

- Fork the repository
- Create a new branch for your feature or bug fix
- Commit your changes and push your branch to your fork
- Open a pull request with a clear description of your changes

We appreciate bug reports, feature requests, and any other form of contribution. Your help makes this project better for everyone.

## Installation

To use phpQuery in your project, you can install it via Composer:

```bash
composer require php-query/php-query
```

## Usage

Here's a simple example of how you can use phpQuery in your PHP code:

```php
// Include the Composer autoloader
require 'vendor/autoload.php';

// Create a new phpQuery object
$html = '<div><p>Hello, <span>world!</span></p></div>';
$doc = phpQuery::newDocument($html);

// Manipulate the DOM using jQuery-like syntax
$text = $doc['div p span']->text(); // Retrieve the text content
echo $text; // Output: world!
```

For more detailed documentation and examples, please refer to the [wiki](https://github.com/your-vendor-name/phpquery/wiki).

## Get in Touch

If you have any questions, suggestions, or feedback, feel free to open an issue or reach out to us via email at [your-email@example.com](mailto:your-email@example.com).

---

**Note:** This repository is a community-driven effort to make phpQuery compatible with PHP 8.x. While we strive for compatibility and functionality, please be aware that this version may have ongoing developments and improvements.
