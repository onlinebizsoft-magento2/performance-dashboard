Performance Dashboard Extension for Magento 2
=====================

The Performance Dashboard Extension by MageHost.pro adds a screen to the Magento Store Admin called "Performance Dashboard". In this screen you get a clear overview of areas where the performance of your Magento 2 can be improved.

# Install #

```
composer config repositories.magehost_performance-dashboard vcs git@github.com:magehost/performance-dashboard.git
composer require magehost/performance-dashboard --no-update
composer update magehost/performance-dashboard
php bin/magento module:enable MageHost_PerformanceDashboard
php bin/magento setup:upgrade
php bin/magento setup:di:compile
```

# Usage #

* In Admin go to _System > Tools > Performance Dashboard_.

# Uninstall #
```
composer remove magehost/performance-dashboard
php bin/magento setup:upgrade
php bin/magento setup:di:compile
```

# Screenshot #
![screenshot](https://raw.githubusercontent.com/magehost/performance-dashboard/master/doc/screenshot.png)

# Description #
Using our experience as [Magento Hosting professionals](https://magehost.pro) we created a list of best-practises for a high performance Magento 2 setup.
Based on this list we have created a dashboard which automatically tests these various config settings and other choices.
One of the checks logs CMS and Catalog pages which can't be cached in full-page-cache because of `cacheable="false"`.
