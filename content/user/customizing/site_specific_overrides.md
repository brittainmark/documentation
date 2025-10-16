---
title: Site Specific Overrides 
description: More ways to customize your cart's behavior without modifying core files
category: customizing
weight: 10
---

Note: This document is for the storefront side site specific overrides. [Here are the Admin site specific overrides](/user/admin/site_specific_overrides/). 

## Setting Overrides 

Starting in Zen Cart 1.5.8, a file called `includes/extra_datafiles/dist-site_specific_overrides.php` is provided.  

Copy this file to 

`includes/extra_datafiles/site_specific_overrides.php`

and customize to taste. 

Many behaviors can be enabled or disabled by this file, such as:

- displaying the [About Us](/user/storefront_pages/about_us/) link in the Information sidebox (```$flag_show_about_us_sidebox_link```).
- displaying the [Accessibility Page](/user/storefront_pages/accessibility/) link in the Information sidebox (```$flag_show_accessibility_sidebox_link```).
- displaying the [Brands page](/user/storefront_pages/brands/) link in the Information sidebox (```$flag_show_brand_sidebox_link```).
- (developers) whether to enable debug on the `zcDate` class (```$zen_date_debug```).
- (developers) whether to bypass loading string-matches of legacy language files (```'NO_LANGUAGE_SUBSTRING_MATCH'```)  (see [Substring Matching](/dev/languages/158_order_language_files/) for details).
- (developers) whether to disable loading the [Font Awesome](/user/template/font_awesome/) v4 shim if backwards compatibility is not needed (```$disableFontAwesomeV4Compatibility```).
- whether a product's additional images should be displayed if the product has no 'main' image defined (```$enable_additional_images_without_main_image```).
- set category counts to count only distinct products: if a product is in two different sub categories of a parent category it will only be counted once (```'COUNT_DISTINCT_PRODUCTS'```).
- for Checkout Shipping, when no shipping method is available, substitute the Continue button with a Contact Us button (```$show_contact_us_instead_of_continue```).
- for Product Listing: enable the legacy sorting by column heading (```$show_table_header_row```).

See the file itself for further details.

Information on the [admin site-specific overrides file](/user/admin/site_specific_overrides/) is also available. 

## Non-Database Setting Overrides 

Starting in Zen Cart 1.5.8, a file called `/includes/init_includes/dist-init_site_specific_non_db_settings.php` is provided.  

Copy this file to 

`/includes/init_includes/init_site_specific_non_db_settings.php`

and customize to taste. The settings that may be altered in this file are listed in the file `includes/init_includes/init_non_db_settings.php`.

## Bootstrap Template Setting Overrides 

Users of the [Bootstrap template](/user/template/bootstrap/) may customize it in the following ways: 

- The [Bootstrap Template site_specific_styles.php file](https://github.com/lat9/ZCA-Bootstrap-Template/wiki/Frequently-Asked-Questions) allows you to modify the template's CSS.
- The [Bootstrap Template site-specific-bootstrap-settings.php file](https://github.com/lat9/ZCA-Bootstrap-Template/wiki/%22Soft%22-Configuration-Settings) allows you to implement some commonly-requested tweaks (Soft Configurations) of the template's behavior.

## Responsive Classic Template Setting Overrides 

Users of the [Responsive Classic template](/user/template/responsive_classic/) may customize it in the following ways: 

- Since Zen Cart 2.0.0, the `site_specific_styles.php` file allows you to modify the template's CSS.  A sample file (`dist-site_specific_styles.php`) is provided since Zen Cart 2.2.0. 

## Related Links 
- [Template Settings](/dev/code/template_settings/) file

