# wso2esb-passwordreset

## For default installations

```
sudo apt-get update
sudo apt-get install ant
** stop wso2esb **
cd <wso2esb>/bin
./chpasswd.sh --db-url "jdbc:h2:repository/database/WSO2CARBON_DB" --db-driver org.h2.Driver --db-username wso2carbon --db-password wso2carbon --username admin
** start wso2esb **
```

## Different DB installations

```
sudo apt-get update
sudo apt-get install ant
** stop wso2esb **
** copy needed driver to repository/components/lib **
cd <wso2esb>/bin
./chpasswd.sh --db-url "jdbc:<db url details>" --db-driver <db driver> --db-username wso2carbon --db-password wso2carbon --username admin
** start wso2esb **
```
