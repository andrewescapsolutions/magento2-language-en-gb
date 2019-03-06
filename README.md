This is an additional fork from cubewebsites/magento2-language-en-gb to allow it to be used on Magento 2.3.x. I've only modified the composer details, credit to their work for everything else.

# Links

* Website: https://github.com/andrewescapsolutions/magento2-language-en-gb

# What's Up With The Fork?

This fork is created from the original for 3 main reasons:

1. The original doesn't install
1. When it does install, it doesn't load
1. When it does load, it turns out that for some reason half the translations are in French!

As well as fixing the above issues, I've also updated a **lot** of the translations to meet my requirements.

## Why Include 3rd Party Themes?

Themes normally contain translation files inside the theme which mostly works fine.  However, for theme translations that are passed to JS (Knockout) Magento won't pick them up from the theme folder and they need to be included in the language pack instead. 

# Installation

## Composer method

```
cd <your magento path>
composer require escapsolutions/magento2-language-en-gb:*
php bin/magento cache:clean
```

To update package

```
cd <your magento path>
composer update escapsolutions/magento2-language-en-gb
php bin/magento cache:clean
```

## Download repository method

Download file: https://github.com/andrewescapsolutions/magento2-language-en-gb/archive/master.zip

```
cd <your magento path>
Create folder your-magento-path/app/i18n/cubewebsites/en_gb and extract zip into path.
php bin/magento cache:clean
```
# Contribute

Feel free to submit updates, corrections and other 3rd-party theme translations and I'll get them added
