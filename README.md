# WooCommerce BGN-EUR Price Display

**Author:** no7r3k  
**Tags:** woocommerce, currency, bgn, eur, conversion, dual-currency    
**Requires PHP:** 7.4  
**Stable tag:** 2.0.1  
**License:** GPLv2  
**License URI:** https://www.gnu.org/licenses/old-licenses/gpl-2.0.html

Display prices in BGN alongside EUR with optional permanent conversion.

---

## Description

**WooCommerce BGN-EUR Price Display** lets you:

- Enter a custom BGN - EUR exchange rate (current official ECB rate shown for reference).  
- Show converted EUR prices on shop, category, and single-product pages.  
- Choose from multiple display formats (append, prepend, show only EUR).  
- Define decimal precision for both currencies (for conversion).  
- Run a one-click batch conversion of all BGN prices to EUR in your database.  
- (Optional) Switch your store’s **primary** currency to EUR, affecting all WooCommerce calculations (can be used after conversion).

Perfect for Bulgarian retailers who need dual-currency display or full migration to Euro pricing.

---

## Installation

1. Upload the `wc-bgn-eur` folder to your `/wp-content/plugins/` directory, or install via the WordPress plugin installer.  
2. Activate “WooCommerce BGN-EUR Price Display” through **Plugins**.  
3. Navigate to **WooCommerce → Settings → BGN-EUR Price Display** to configure.

---

## Configuration

### Exchange Rate  
Enter your desired BGN - EUR rate (e.g. `1.9559`). The current ECB rate is displayed for convenience.

### Display Options  
- ☑ Show on shop & archive pages  
- ☑ Show on category pages  
- ☑ Show on single product pages  

### Price Display Format  
Select how EUR appears:  
- **Append:** `12.50 лв (6.39 €)`  
- **Prepend:** `(6.39 €) 12.50 лв`  
- **Show only EUR:** `6.39 €`  

### Decimal Places  
Set precision for both BGN and EUR values.

### Conversion Batch Size  
Choose how many products to process per AJAX batch. Lower values reduce timeout risk on shared hosting.

### Primary Currency  
- ☐ Use EUR as primary currency (affects all WooCommerce pricing, shipping, tax).  
> **Warning:** Permanently changes your shop’s base currency.

### Price Conversion Tools  
- **Get Statistics:** Shows count of products pending conversion.  
- **Download Backup:** Always back up before converting (not functional at the moment).  
- **Convert BGN - EUR:** Overwrite BGN prices with EUR equivalents.  
- **Convert EUR - BGN:** Revert (uses the same rate; no further edits needed).

---

## Frequently Asked Questions

**Is the batch conversion reversible?**  
Somewhat—you can convert back via “Convert EUR - BGN,” but always back up your database first.

**Can I auto-update rates?**  
No. The exchange rate is set manually; ECB publishes a fixed reference rate.

**Will taxes and shipping update?**  
Only if “Use EUR as primary currency” is enabled. You may also need to update tax rules/prices separately.

---

## Screenshots
![Plugin](https://github.com/no7r3k/woocommerce-bgn-to-eur/blob/6252ab3dcbbefbbaf9016b3b6a6c11fdf36e58d2/BGNtoEUR.png)
1. Settings page with exchange-rate input  
2. Display options checkboxes  
3. Batch conversion tools panel  

---

## Changelog

### 2.0.1
- Minor UI tweaks  
- Bug fixes  

### 2.0.0
- Major refactor; added prepend/replace formats  
- Improved AJAX batching  
- Introduced “Use EUR as primary currency”  

### 1.0.0
- Initial release  

---

## License

This plugin is licensed under the **GNU GENERAL PUBLIC LICENSE v2.0**  
