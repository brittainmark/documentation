---
title: Other Topics 
description: Other information about SEO in Zen Cart 
category: seo
weight: 1000
---

## Disabled Product Status for Search Engines
Zen Cart has a configuration setting called [DISABLED_PRODUCTS_TRIGGER_HTTP200](/user/admin_pages/configuration/configuration_stock/#disabled_product_status_for_search_engines).  The default behavior of the product is to not show a product info page for a disabled product; this switch allows the behavior to be changed.  Users who set this value to `true` may require template changes to ensure customers do not actually buy disabled products. See [this page](https://github.com/zencart/zencart/discussions/6165) for more information.

## SEO URLs 

The phrase "SEO URLs" is sometimes used to describe the process of rewriting URLs to contain keywords.   Some experts believe this process improves your search engine rankings and is thus beneficial to your site. 

The default installation of Zen Cart does not create "SEO URLs" (URLs that are self-describing).  Some plugins are available to do this:

- [Ultimate SEO URLs](https://www.zen-cart.com/downloads.php?do=file&id=132) - This plugin is well supported by @lat9 and is the recommended solution for people who want a URL rewriter.

- [CEON URI Mapping](https://github.com/JSWebSteve/Ceon-URI-Mapping-V5.1.0) - Since the author's death, support for this plugin has been inconsistent.  Note that CEON URI Mapping does not automatically add mappings for EXISTING Categories/Products/Manufacturers/EZ-Pages.  You must either edit these items one by one or purchase the URI Mappings Manager from CEON if you are using a pre-existing database.  

The plugin [Simple SEO URLs](https://www.zen-cart.com/downloads.php?do=file&id=1754) is no longer supported.


## Images and SEO
Image alt text is used by search engines and can improve your SEO.  Providing alt text is also an important part of making your site accessible.  See [Alt Text](/user/accessibility/concerns/alt_text/) for more details. 
