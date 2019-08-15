# WP-CLI WooCommerce to EDD Migration Script

Handles migrating WooCommerce to Easy Digital Downloads (Including support for Subscriptions and API Keys).

## Requirements

WP-CLI WooCommerce to EDD Migration Script requires [WooCommerce](https://wordpress.org/plugins/woocommerce/) and [Easy Digital Downloads](https://wordpress.org/plugins/easy-digital-downloads/) to be active.

To migrate WooCommerce data to Easy Digital Downloads, [you'll need to have the ability to run WP-CLI commands in your environment](http://wp-cli.org/).

## Installation ##

This section describes how to install the plugin and get it working.

1. Upload `woocommerce-to-edd-migration` to the `/wp-content/plugins/` directory.
1. Activate the plugin through the 'Plugins' menu in WordPress.

To activate the plugin using WP-CLI you can run this command.

```
$ wp plugin activate wp-cli-woo-to-edd-migration
```

## Migrating WooCommerce data to Easy Digital Downloads

After installing and activating the plugin, you'll need to migrate products, product categories (taxonomies), coupons and orders.

The way to accomplish this is via [WP-CLI](http://wp-cli.org/), and the plugin ships with a number of commands to help.

### Migrate products from WooCommerce

The `migrate_products` command will migrate products from WooCommerce into download in EDD.

```
$ wp migrate_woo migrate_products
```

### Migrate product categories from WooCommerce

The `migrate_taxonomies` command will migrate product categories from WooCommerce into download categories and tags in EDD.

```
$ wp migrate_woo migrate_taxonomies
```

### Migrate coupons from WooCommerce

The `migrate_coupons` command will migrate coupons from WooCommerce into discount codes in EDD.

```
$ wp migrate_woo migrate_coupons
```

### Migrate order data WooCommerce

The `migrate_orders` command will migrate orders from WooCommerce into payments in EDD.

```
$ wp migrate_woo migrate_orders
```
