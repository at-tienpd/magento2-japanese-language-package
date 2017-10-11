# Magento2-japanese-language-package for Asiantech First Theme (Magento ver. 2.1.7)

# Create store view for Japan store

1. STORE >> Settings >> All Stores >> Create Store View 
	+ Name       : Japanese
	+ Code       : japanese
	+ Status     : Enabled
	+ Sort Order : 1
2. Save Store View

# Run terminal

php bin/magento indexer:reindex

# Set locale and currency for Japan store

1. STORE >> Settings >> Configuration
2. Set Store View to Japanese
3. GENERAL >> General
4. Set Country Options >> Default Country is Japan
5. Set Locale Options >> Locale is Japanese(Japan)
6. GENERAL >> Currency Setup >> Currency Options
7. Set Default Display Currency is Japanese Yen
8. Set Allowed Currencies is Japanese Yen

# Set currency rate for Japan store

1. STORE >> Currency >> Currency Rates
2. Click Import
3. Click Save Currency Rates

# Download package 

Rename magento2-japanese-language-package to i18n and set place in app folder

# Run terminal

php bin/magento setup:static-content:deploy ja_JP

Last one you should be login admin and edit categories and products to Japanese.

# License

TIEN © 2017 Happy coding

