# WP-CLI WooCommerce to EDD Migration Script

Handles migrating WooCommerce to Easy Digital Downloads (Including support for Subscriptions and API Keys).

## Requirements

WP-CLI WooCommerce to EDD Migration Script requires [WooCommerce](https://wordpress.org/plugins/woocommerce/) and [Easy Digital Downloads](https://wordpress.org/plugins/easy-digital-downloads/) to be active.

To migrate WooCommerce data to Easy Digital Downloads, [you'll need to have the ability to run WP-CLI commands in your environment](http://wp-cli.org/).

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

## Contributing

If you're interested in contributing to the development of the plugin or need to report an issue, please [see the contributing guidelines for the project](https://github.com/sebastianmoran-mainwp/woocommerce-to-edd-migration/CONTRIBUTING.md).
