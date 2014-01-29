=== Plugin Name ===
Contributors: pomegranate
Tags: woocommerce, print, pdf, bulk, packing slips, invoices, delivery notes, invoice, packing slip, export, email
Requires at least: 3.5 and WooCommerce 2.0
Tested up to: 3.8 and WooCommerce 2.1
Stable tag: 1.1.5
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Create, print & automatically email PDF invoices & packing slips for WooCommerce orders.

== Description ==

This WooCommerce extension automatically adds a PDF invoice to the order confirmation emails sent out to your customers. Includes a basic template (additional templates are available from [WP Overnight](https://wpovernight.com/downloads/woocommerce-pdf-invoices-packing-slips-premium-templates/)) as well as the possibility to modify/create your own templates. In addition, you can choose to download or print invoices and packing slips from the WooCommerce order admin.

= Main features =
* Export invoices or packing slips to PDF (individually or in bulk)
* Automatically attach invoice PDF to order confirmation email
* Users can download their invoices from the My Account page
* Available in: Dutch, English, French, German, Italian & Spanish

= Fully customizable =
In addition to a number of default settings (including a custom header/logo) and several layout fields that you can use out of the box, the plugin contains HTML/CSS based templates that allow for customization & full control over the PDF output.

* Insert customer header image/logo
* Modify shop data / footer / disclaimer etc. on the invoices & packing slips
* Select paper size (Letter or A4)
* Translation ready

If you want more control over the invoice numbers, we recommend that you also install the (free) [WooCommerce Sequential Order Numbers plugin](http://wordpress.org/plugins/woocommerce-sequential-order-numbers/)

== Installation ==

= Automatic installation =
Automatic installation is the easiest option as WordPress handles the file transfers itself and you don't even need to leave your web browser. To do an automatic install of WooCommerce PDF Invoices & Packing Slips, log in to your WordPress admin panel, navigate to the Plugins menu and click Add New.

In the search field type "WooCommerce PDF Invoices & Packing Slips" and click Search Plugins. You can install it by simply clicking Install Now. After clicking that link you will be asked if you're sure you want to install the plugin. Click yes and WordPress will automatically complete the installation. After installation has finished, click the 'activate plugin' link.

= Manual installation via the WordPress interface =
1. Download the plugin zip file to your computer
2. Go to the WordPress admin panel menu Plugins > Add New
3. Choose upload
4. Upload the plugin zip file, the plugin will now be installed
5. After installation has finished, click the 'activate plugin' link

= Manual installation via FTP =
1. Download the plugin file to your computer and unzip it
2. Using an FTP program, or your hosting control panel, upload the unzipped plugin folder to your WordPress installation's wp-content/plugins/ directory.
3. Activate the plugin from the Plugins menu within the WordPress admin.

== Frequently Asked Questions ==

= How do I create my own custom template? =

Copy the files from `woocommerce-pdf-invoices-packing-slips/templates/pdf/Simple/` to `yourtheme/woocommerce/pdf/yourtemplate` and customize them there. The new template will shop up as 'yourtemplate' (the folder name) in the settings panel.

= Where can I find more templates? =

Go to [wpovernight.com](https://wpovernight.com/downloads/woocommerce-pdf-invoices-packing-slips-premium-templates/) to checkout more templates! These include templates with more tax details and product thumbnails. Need a custom templates? Contact us at support@wpovernight.com for more information.

= My language is not included, how can I contribute? =

This plugin is translation ready, which means that you can translate it using standard WordPress methods.

1. Download POEdit at (http://www.poedit.net/download.php)
2. Open POEdit
3. File > New from POT
4. Open wpo_wcpdf.pot (from `woocommerce-pdf-invoices-packing-slips/languages/`)
5. A popup will ask you for your language
6. This step is a bit tricky, configuring the plurals. Somehow the settings can't be copied from the pot. Go to Catalogue > Preferences. Then enter nplurals=2; plural=n != 1; in the custom expression field
7. Enter the translations. invoice and packing-slip now have two translation fields, single & plural. Note that this is a filename, so replace spaces with a - just to be sure!
8. Save as `wpo_wcpdf-xx_XX.po`, where you replace xx_XX with your language code & country code suffix (da_DK, pl_PL, de_DE etc.)

= Fatal error: Allowed memory size of ######## bytes exhausted (tried to allocate ### bytes) =

This usually only happens on batch actions. PDF creation is a memory intensive job, especially if it includes several pages with images. Go to WooCommerce > System Status to check your WP Memory Limit. We recommend setting it to 128mb or more.

== Screenshots ==

1. General settings page
2. Template settings page
3. Simple invoice PDF
4. Simple packing slip PDF

== Changelog ==

= 1.1.5 =
* Feature: German translations added - thanks Christian!
* Fix: dompdf 0.6.0 proved to be less stable, so switching back to beta3 for now.

= 1.1.4 =
* Fix: Template paths on windows servers were not properly saved (stripslashes), resulting in an empty output.

= 1.1.3 =
* Feature: PDF engine (dompdf) updated to 0.6.0 for better stability and utf-8 support.
* Tweak: Local server path is used for header image for better compatibility with server settings.
* Fix: several small bugs.

= 1.1.2 =
* Feature: Totals can now be called with simpler template functions
* Feature: Italian translations - thanks max66max!
* Tweak: improved memory performance

= 1.1.1 =
* Feature: French translations - thanks Guillaume!

= 1.1.0 =
* Feature: Fees can now also be called ex. VAT
* Feature: Invoices can now be downloaded from the My Account page
* Feature: Spanish translation & POT file included
* Fix: ternary statements that caused an error

= 1.0.1 =
* Tweak: Packing slip now displays shipping address instead of billing address
* Tweak: Variation data is now displayed by default

= 1.0.0 =
* First release