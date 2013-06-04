Stripe Example
======

Drupal module for Stripe

Installing
1) Install the module in drupal's /sites/all/modules
2) create a lib folder inside the stripe module (ex:/sites/all/modules/stripe/lib)
3) clone the stripe php library from within the stripe/lib folder you just created.
  - git clone https://github.com/stripe/stripe-php.git
4) Now the stripe library should be at /sites/all/modules/stripe/lib/stripe-php
5) Enable the stripe module with drush en stripe, or through the interface.

Configuration
In order to submit credit cards to strip you will need to define your keys.
1) Navigate to /#overlay=admin/config and click "Stripe" under the web services heading.
2) Enter you Secret Key and Publishable key for testing and close the overlay.
3) Navigate to the checkout page under the default drupal navigation.
4) Submit your billing information and credit card information.

ToDos
1) Register the stripe library using the Library 2.0 API and hook_library_info().
2) Save the billing and some transaction information in a new table schema created in install.
3) Provide a viewable report with sorting and filtering abilities.
4) Further enhance testing of the module.
