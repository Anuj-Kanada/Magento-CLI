# Important Command For Magento Development

- ddev magento setup:upgrade or s:up
- ddev mageno cache:flush 
- ddev magento cache:clean 
- ddev magento setup:di:compile
- ddev magento static:content:deploy
- ddev magento sampladata:deploy
- ddev magento sampledata:remove
- ddev magento samplesata:reset
- php bin/magento setup:db-declaration:generate-whitelist --module-name=YourModule_Name
- php bin/magento module:enable vendor_module
- ddev magento catalog:images:resize-a
- ddev magento catalog:images:resize <theme_dir>
- php bin/magento admin:user:unlock username
- php bin/magento setup:upgrade --keep-generated  -> Setup upgrades without removing pub/static files using the CLI:

# To enable developer mode and error report :
- php bin/magento deploy:mode:set developer
- Go to pub/errors/local.xml.sample => rename this file with : local.xml
- Go to app/bootstrap.php => Line no 14 ini_set('display_errors', 1); Remove # from this line and save file.
