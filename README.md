# magento2-catalog-import
Magento console command for importing catalog files.

## Install
```bash
composer require wilkesystems/magento2-catalog-import:dev-master
php bin/magento module:enable WilkeSystems_CatalogImport
php bin/magento setup:upgrade
```

## Usage
```bash
php bin/magento catalog:import [-i|--images_path[="..."]] [-b|--behavior[="..."]] csv_file
```

- `--images_path`: (default `pub/media/catalog/product`) must be a relative path starting from your Magento2 project root
- `--behavior`: (default `append`) possible values: append, add_update, replace, delete
- csv_file: could be a relative or an absolute path to a valid CSV file
