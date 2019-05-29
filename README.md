# Magento 2 Coding standard procedure

###### *NOTE: this is a fork from official module magento/magento-coding-standard and modified to work with Magento 2.3 and PHP7.2*

## 1. install php-code-sniffer and magento-coding-standard 
### Requirements
- required php version for your project (7.1, 7.2)
- composer https://getcomposer.org/

### Install patched `magento-coding-standard` module

I've created a patched version of module `magento-coding-standard` , you can install it using command below

```
# install the module
$ composer require --dev isevenr/magento-coding-standard dev-master

# include path for phpcs command line tool
$ php vendor/bin/phpcs --config-set  installed_paths ../../isevenr/magento-coding-standard
```

## 2. before commiting code ,  use phpcs and magento-coding-standard check for issue and fix

you can run phpcs from the command-line to analyse your code like below
```
# Analyse your new module3
$ php vendor/bin/phpcs --standard=Magento2 app/code/MyAwesomeExtension

# Analyse new custom code you just wrote
$ php vendor/bin/phpcs --standard=Magento2 path/to/my/new/custom/code
```
