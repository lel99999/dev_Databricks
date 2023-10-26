# dev_Databricks
Databricks workspace and Notes

#### JDBC Link v2.6.34
- [JDBC Driver](https://databricks-bi-artifacts.s3.us-east-2.amazonaws.com/simbaspark-drivers/jdbc/2.6.34/DatabricksJDBC42-2.6.34.1058.zip) <br/>
- Install into /usr/lib64/databricks <br/>
  
#### ODBC Link v2.7.5
- [ODBC Drivers](https://www.databricks.com/spark/odbc-drivers-download) <br/>
  - [Linux(RPM)](https://databricks-bi-artifacts.s3.us-east-2.amazonaws.com/simbaspark-drivers/odbc/2.7.5/SimbaSparkODBC-2.7.5.1012-LinuxRPM-64bit.zip) <br/>
  - [Windows](https://databricks-bi-artifacts.s3.us-east-2.amazonaws.com/simbaspark-drivers/odbc/2.7.5/SimbaSparkODBC-2.7.5.1012-Windows-64bit.zip) <br/>
  - Installs into /opt/simba/spark <br/>

#### ODBC Configuration odbc.ini
[Databricks_SQLWarehouse]
Driver          = /opt/simba/spark/lib/64/libsparkodbc_sb64.so
Description     = Simba Spark ODBC Driver DSN
HOST            = hostname.cloud.databricks.com
PORT            = 443
Schema          = default
SparkServerType = 3
AuthMech        = 3
UID             = token
PWD             = <personal-access-token>
ThriftTransport = 2
SSL             = 1
HTTPPath        = /sql/1.0/warehouses/fa12345678f8b014
