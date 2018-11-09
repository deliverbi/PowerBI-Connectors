# PowerBI-Connectors Custom ODBC Direct Query Presto refined
PowerBI Custom ODBC Direct Query Connector


We were stuck on a project as a client needed Direct Query ability to Presto via a ODBC Connection.

The Connector supports Presto & Hive ODBC aswell as all other ODBC targets. Its quite a simple connector that incorporates a few data type mappings.

1. Download the Connector .mez file.
a
2. Under your documents folder / Create a New Folder called "Power BI Desktop" within this folder Create a folder called "Custom Connectors"

3. Copy the downloaded .mez connector to the newly created folder Custom Connectors above.

4. Within PowerBI enable Custom Connectors - New Version Under Security tab enable -- Old version under Privacy tab.

5. Restart PowerBI 

6. Your new Custom Connector will be visible


# Using the Connector

Create your ODBC Connection within your windows ODBC Manager - Copy the DSN Name "This is the name of your connection".

DSN is the only mandatory parameter within powerbi along with any username and password.

Please use at your own risk - Works ok for our reporting requirements.

Presto Notes ****

BigInt - Powerbi issues with BigInt -- Fixed on 09/11/2018 release
Decimal - Working Ok - Preferes Double as some glitches on Filters within POWERBI. (Unrelated to Connector) Fixed on 09/11/2018 release


