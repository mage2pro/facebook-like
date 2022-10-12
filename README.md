The «[**Facebook Like & Share**](https://mage2.pro/c/extensions/facebook-like)» module for Magento 2 shows the Facebook's «Like» and «Share» buttons on the frontend product pages.  
The module is **free** and **open source**.

![](https://mage2.pro/uploads/default/original/1X/3782ec58041a937703bb61bdda5b1d8c028da5e6.png)

## How to install
[Hire me in Upwork](https://www.upwork.com/fl/mage2pro), and I will: 
- install and configure the module properly on your website
- answer your questions
- solve compatiblity problems with third-party checkout, shipping, marketing modules
- implement new features you need 

### 2. Self-installation
```
bin/magento maintenance:enable
rm -f composer.lock
composer clear-cache
composer require mage2pro/facebook-like:*
bin/magento setup:upgrade
bin/magento cache:enable
rm -rf var/di var/generation generated/code
bin/magento setup:di:compile
rm -rf pub/static/*
bin/magento setup:static-content:deploy -f en_US <additional locales>
bin/magento maintenance:disable
```

## How to update
```
bin/magento maintenance:enable
composer remove mage2pro/facebook-like
rm -f composer.lock
composer clear-cache
composer require mage2pro/facebook-like:*
bin/magento setup:upgrade
bin/magento cache:enable
rm -rf var/di var/generation generated/code
bin/magento setup:di:compile
rm -rf pub/static/*
bin/magento setup:static-content:deploy -f en_US <additional locales>
bin/magento maintenance:disable
```