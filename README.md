=== WooCommerce BGN-EUR Price Display ===
Contributors: no7r3k
Tags: woocommerce, currency, bgn, eur, conversion, dual-currency
Requires at least: 5.0
Tested up to: 6.4
Requires PHP: 7.4
WC requires at least: 5.0
WC tested up to: 8.5
Stable tag: 2.0.1
License: LGPLv3
License URI: https://www.gnu.org/licenses/lgpl-3.0.html

Display prices in BGN alongside EUR prices with optional permanent conversion.

== Description ==

WooCommerce BGN-EUR Price Display lets you:

* Enter a custom BGN to EUR exchange rate (the current official rate is shown for reference).  
* Show converted EUR prices on shop, category, and single-product pages.  
* Choose from multiple display formats (append, prepend, show only EUR).  
* Define decimal precision for both currencies (for conversion).  
* Run a one-click batch conversion of all BGN prices to EUR in your database.  
* (Optional) Switch your store’s **primary** currency to EUR, affecting all WooCommerce calculations (can be used after conversion).

Perfect for Bulgarian retailers who need dual-currency display or full migration to Euro pricing.

== Installation ==

1. Upload the `wc-bgn-eur` folder to `/wp-content/plugins/`, or install via the WordPress plugin installer.  
2. Activate "WooCommerce BGN-EUR Price Display" through **Plugins**.  
3. Navigate to **WooCommerce - Settings - BGN-EUR Price Display** to configure.

== Configuration ==

=== Exchange Rate ===  
– Enter your desired BGN to EUR rate (e.g. `1.9559`). The current ECB rate is displayed for convenience.

=== Display Options ===  
☑ Show on shop & archive pages  
☑ Show on category pages  
☑ Show on single product pages

=== Price Display Format ===  
Select how EUR appears:  
- **Append:** `12.50 лв (6.39 €)`  
- **Prepend:** `(6.39 €) 12.50 лв`  
- **Show only EUR:** `6.39 €`

=== Decimal Places ===  
Set precision for both BGN and EUR values.

=== Conversion Batch Size ===  
Choose how many products to process per AJAX batch. Lower values reduce timeout risk on shared hosting.

=== Primary Currency ===  
☐ Use EUR as primary currency (affects all WooCommerce pricing, shipping, tax).  
! Permanently changes your shop’s base currency. !

=== Price Conversion Tools ===  
- **Get Statistics:** Shows count of products pending conversion.  
- **Download Backup:** Always back up before converting, but does not work at the moment...
- **Convert BGN - EUR:** Overwrite BGN prices with EUR equivalents.  
- **Convert EUR - BGN:** Revert (uses the same rate and no further edits are needed).

== Frequently Asked Questions ==

= Is the batch conversion reversible? =  
Somewhat, as you can convert back the product prices. Either way, you should create a database backup beforehand.

= Can I auto-update rates? =  
No, but the exchange rate is fixed with the ECB and would not change. 

= Will taxes and shipping update? =  
Only if "Use EUR as primary currency" is enabled, but you might have to edit the prices of your taxes separately.

== Screenshots ==

1. Settings page with rate input  
2. Display options checkboxes  
3. Batch conversion panel

== Changelog ==

= 2.0.1 =  
* Minor UI tweaks
* Bug fixes
  
= 2.0.0 =  
* Major refactor; added replace/prepend formats  
* Improved AJAX batching  
* Introduced “Use EUR as primary currency”  

= 1.0.0 =  
* Initial release

== License ==

This plugin is licensed under the GNU Lesser General Public License v3.0  
