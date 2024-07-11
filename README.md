# Important Command For Magento Development

- ddev magento s:up
- ddev mageno cache:flush 
- ddev magento cache:clean 
- ddev magento setup:di:compile
- ddev magento static:content:deploy
- ddev magento sampladata:deploy
- php bin/magento setup:db-declaration:generate-whitelist --module-name=YourModule_Name
# To enable developer mode and error report :
- php bin/magento deploy:mode:set developer
- Go to pub/errors/local.xml.sample => rename this file with : local.xml
- Go to app/bootstrap.php => Line no 14 ini_set('display_errors', 1); Remove # from this line and save file.
