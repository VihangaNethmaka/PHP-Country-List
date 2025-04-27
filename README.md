# Country Data (PHP)

A comprehensive PHP array containing a list of countries with their names, ISO 3166-1 alpha-2 codes, international dial codes, and flag emojis.

## Features

* Includes a wide range of countries.
* Data is structured as an associative array for easy access.
* Sorted alphabetically by country name.
* Provides essential information for web development tasks like dropdown menus, phone number validation, and displaying country-specific information.

## Usage

1.  **Installation (via Composer - Recommended):**

    If you're using Composer in your PHP project, you can add this repository as a dependency.

    ```bash
    composer require your-github-username/country-data-php
    ```

    Replace `your-github-username/country-data-php` with your actual GitHub username and repository name.

    Then, you can include the data in your PHP code:

    ```php
    <?php

    require 'vendor/autoload.php';

    // Assuming the file is directly in the root after Composer install
    // $countries = require 'countries.php';

    // If the file is in the data directory
    $countries = require 'vendor/your-github-username/country-data-php/data/countries.php';

    // Now you can work with the $countries array
    print_r($countries[0]); // Output: Array ( [name] => Afghanistan [code] => AF [dial_code] => +93 [flag] => 🇦🇫 )

    ?>
    ```

2.  **Manual Installation:**

    Alternatively, you can directly download the `countries.php` file and include it in your project:

    ```php
    <?php

    require 'path/to/your/downloaded/countries.php';

    // Now you can work with the $countries array
    print_r($countries[1]); // Output: Array ( [name] => Albania [code] => AL [dial_code] => +355 [flag] => 🇦🇱 )

    ?>
    ```

## Data Structure

The `$countries` array is an indexed array of associative arrays. Each inner array represents a country and has the following keys:

* `name`: The common name of the country (string).
* `code`: The ISO 3166-1 alpha-2 country code (string).
* `dial_code`: The international dialing code (string).
* `flag`: The flag emoji (string).

## Contributing

If you find any errors, omissions, or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License

[Specify your chosen license here, e.g., MIT License](LICENSE)

## Author

[Your Name or GitHub Username]
