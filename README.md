# dev_Databricks
Databricks workspace and Notes


#### DBUTILS Reference
- [https://docs.databricks.com/en/dev-tools/databricks-utils.html](https://docs.databricks.com/en/dev-tools/databricks-utils.html) <br/>

#### CLI
Legacy: <br/>
- [https://docs.databricks.com/en/archive/dev-tools/cli/index.html](https://docs.databricks.com/en/archive/dev-tools/cli/index.html) <br/>
- [https://docs.databricks.com/en/archive/dev-tools/dbx/dbx.html](https://docs.databricks.com/en/archive/dev-tools/dbx/dbx.html) <br/>

Update: <br/>
- [https://docs.databricks.com/en/dev-tools/cli/install.html](https://docs.databricks.com/en/dev-tools/cli/install.html) <br/>

#### API Docs
- [https://docs.databricks.com/en/reference/api.html](https://docs.databricks.com/en/reference/api.html) <br/>

#### Authentication for Databricks Automation
- [https://docs.databricks.com/en/dev-tools/auth.html](https://docs.databricks.com/en/dev-tools/auth.html) <br/>

#### JDBC Link v2.6.34
- [JDBC Driver](https://databricks-bi-artifacts.s3.us-east-2.amazonaws.com/simbaspark-drivers/jdbc/2.6.34/DatabricksJDBC42-2.6.34.1058.zip) <br/>
- Install into /usr/lib64/databricks <br/>
  
#### ODBC Link v2.7.5
- [ODBC Drivers](https://www.databricks.com/spark/odbc-drivers-download) <br/>
  - [Linux(RPM)](https://databricks-bi-artifacts.s3.us-east-2.amazonaws.com/simbaspark-drivers/odbc/2.7.5/SimbaSparkODBC-2.7.5.1012-LinuxRPM-64bit.zip) <br/>
  - [Windows](https://databricks-bi-artifacts.s3.us-east-2.amazonaws.com/simbaspark-drivers/odbc/2.7.5/SimbaSparkODBC-2.7.5.1012-Windows-64bit.zip) <br/>
  - Installs into /opt/simba/spark <br/>

#### ODBC Configuration odbc.ini 
[Databricks_SQLWarehouse] <br/>
Driver          = /opt/simba/spark/lib/64/libsparkodbc_sb64.so <br/>
Description     = Simba Spark ODBC Driver DSN <br/>
HOST            = hostname.cloud.databricks.com <br/>
PORT            = 443 <br/>
Schema          = default <br/>
SparkServerType = 3 <br/>
AuthMech        = 3 <br/>
UID             = token <br/>
PWD             = <personal-access-token> <br/>
ThriftTransport = 2 <br/>
SSL             = 1 <br/>
HTTPPath        = /sql/1.0/warehouses/fa12345678f8b014 <br/>
