# Cookie Information CMP variable template for Google Tag Manager

The variable template returns the consent state (`boolean`) for any of the specified cookie categories:
* `cookie_cat_necessary`
* `cookie_cat_functional`
* `cookie_cat_marketing`
* `cookie_cat_statistic`
* `cookie_cat_unclassified`


The template retrieves the consent state from the following two sources (in that order):
1. `CookieInformationConsent` cookie
2. `CookieInformation` JS API (window object)

The variable will return `false` if no consent decision has been made yet or consent has been denied for the given cookie category. `True` will be returned if consent has been granted for the given cookie category.

