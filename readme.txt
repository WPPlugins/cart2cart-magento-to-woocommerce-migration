=== Cart2Cart: Magento to WooCommerce Migration   ===
Contributors: cart2cart
Tags: magento to woocommerce, magento to woocommerce migration, migrate magento to woocommerce
Requires at least: 3.5.1
Tested up to: 4.7.4
Stable tag: 4.0
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html 
Plugin helps to migrate all data from Magento to WooCommerce automatically with no programming skills required.

== Description ==
**Supported WooCommerce versions: 1.1.x – 1.6.x, 2.x, 3.x**
**Supported Magento versions: 1.1.x - 2.x CE (1.1 - 1.3 from only), 1.6.x - 1.14.x, 2.x EE**

The plugin will help you to migrate all your data from Magento to WooCommerce automatically. You will be able to transfer products, customers, orders with all corresponding information accurately and effortlessly. 

**The plugin offers 2 migration options**

1. Free Demo migration — lets you perform migration of products, orders, customers and categories in limited quantity (up to 10 entities each) for test purposes.
1. Full Migration — lets you perform UNLIMITED migration of products, orders, customers, categories, variants, attributes and other related entities. Full Migration price starts at $69 and may vary depending on the number of transferable entities and additional options chosen.

= The following entities can be moved from Magento to WooCommerce:
 =
* Products, product images, product extra fields, product attributes, product variants
* Categories, category images 
* Customers, customer shipping address, customer billing address 
* Orders, order statuses

= Features of Automated Migration with Cart2Cart:
 =
- **Simple** - no programming skills required, simply follow a step by step instruction.
- **Fast** - the time of migration depends on a quantity of entities you wish to move and takes a few hours. 
- **Free Demo** - up to 10 entities will be moved for free
- **Support** - contact support team via live chat, phone or ticket at any convenient time.

**Note.** *Plugin supports entities migration only, Magento theme won’t be converted into WooCommerce theme.This plugin installs connection bridges at your Magento and WooCommerce, which is needed for data interaction between two platforms. Upon activation, you’ll be redirected to Cart2Cart website in order to launch the conversion.*

= Steps to Take before Migration =
1. Install WooCommerce and make sure that Magento and WooCommerce stores are available online.
1. Have Magento store FTP access details at hand (host, username, password) - you use them to install connection bridge on Magento.

 

== Installation ==

1. Download the plugin zip file
1. Extract plugin zip file to your PC
1. Upload extracted file to wp-content/plugin directory
1. Go to Admin -> Go to Admin -> Plugins, find “Cart2Cart Magento to WooCommerce Migration” and click Activate
1. You’ll be redirected to Cart2Cartwebsite in order to complete your migration

== Frequently Asked Questions ==
= What is Cart2Cart? =
Cart2Cart is a shopping cart migration service which allows automated data transfer from one platform to another. Currently service supports migration from/to [70+ most popular shopping carts](http://www.shopping-cart-migration.com/supported-carts). Main beneficial sides for e-merchants are:

* No technical skills required. Since the process is fully automated, there is no need to have high level of programming skills. Intuitive [migration Wizard](http://www.shopping-cart-migration.com/quick-demo-tour) will help to perform a straightforward migration.
* Cart2Cart requires no software installation. The migration is performed on Amazon Elastic Cloud servers. The data migration is performed with the help of connection bridge, which is installed for source and target shopping carts and makes the integration possible.

* Cart2Cart provides a possibility to migrate products, customers,orders with all corresponding data to a desirable shopping cart.

* Flexible pricing system allows to pay only for entities, which are really migrated. The price of migration can be calculated with the help of [Online Estimator](https://app.shopping-cart-migration.com/estimator).

* Totally free Demo migration which provides a possibility to try how everything works before launching a Full migration.
If you have some questions, [Support Team](http://support.magneticone.com/index.php?/Tickets/Submit/RenderForm/5) is ready to answer all questions via live chat, phone or ticket at any convenient time.

= Are there any technical requirements for migration performance? =
There are no universal technical requirements for all stores as different platforms have different technical peculiarities. However, there are some recommendation you should consider before setting shopping cart migration.
Recommended PHP configurations:
* memory_limit - 128M (512M for Magento)
* post_max_size - 16M
* max_execution_time - 60
If Suhosin module is installed:
* suhosin.post.max_value_length - 16777216
* suhosin.request.max_value_length - 16777216
Also, it is recommended to switch off the limits for the number of requests to server, as well as firewalls and basic authentication.

= Can I be sure of data security Cart2Cart? =
Cart2Cart performs migration using a separate Amazon EC2 server and all data is deleted after the process has been finished.
Cart2Cart does not migrate client’s credit card information and passwords.
We use secure HTTPS protocol for all connections and only authorized staff has access to the migration process.

= How can I enable Custom fields in WooCommerce? =
Cart2Cart supports migration of Custom fields to WooCommerce 2.x. However, WooCommerce doesn’t display Custom fields by default.
To enable this option you have to:
* go to "store/wp-content/plugins/woocommerce/templates/single-product/tabs"
* find file "additional-information.php"
* add the following code: echo '&lt;table class="shop_attributes"&gt;&lt;tbody&gt;'; foreach(get_post_meta($post-&gt;ID, $key, true) as $key =&gt; $attr) { if(strpos($key, "_") !== 0) { echo '&lt;th&gt;'.$key.'&lt;/th&gt;'; echo '&lt;td&gt;'.array_shift($attr).'&lt;/td&gt;'; echo '&lt;/tr&gt;'; } }	 echo '&lt;/tbody&gt;&lt;/table&gt;';

= Is there a possibility to migrate reviews to WooCommerce? =
Yes, Cart2Cart supports migration of reviews while moving to WooCommerce. Moreover, review ratings will be moved together with reviews.

= Do you migrate multiple languages? =
Yes, Cart2Cart supports migration of multiple languages from Magento to WooCommerce providing a paid WPML module is installed and configured on your WordPress before the data transfer. Please, [read our FAQ](https://www.shopping-cart-migration.com/faq/45-woocommerce/385007-is-multilanguage-migration-to-from-woocommece-possible) for more info.

= Do you migrate customer passwords? =
Yes, there’s a possibility to migrate customer password from Magento to WooCommerce by using a free Cart2Cart: Password Migration plugin. For more info, visit [this page](https://www.shopping-cart-migration.com/cart2cart-password-migration).

== Screenshots ==

1. /assets/screenshot-1.jpg
2. /assets/screenshot-2.jpg 
3. /assets/screenshot-3.jpg
4. /assets/screenshot-4.jpg
5. /assets/screenshot-5.jpg

== Changelog ==

= 1.0 =* Initial commit
