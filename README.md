# PowerBI-Connectors Custom ODBC Direct Query Presto refined
PowerBI Custom ODBC Direct Query Connector


We were stuck on a project as a client needed Direct Query ability to Presto via a ODBC Connection.

The Connector supports Presto & Hive ODBC aswell as all other ODBC targets. Its quite a simple connector that incorporates a few data type mappings.

# Installation

1. Download the Connector .mez file.
a
2. Under your documents folder / Create a New Folder called "Power BI Desktop" within this folder Create a folder called "Custom Connectors"

3. Copy the downloaded .mez connector to the newly created folder Custom Connectors above.

4. Within PowerBI enable Custom Connectors - New Version Under Security tab enable -- Old version under Privacy tab.

5. Restart PowerBI 

6. Your new Custom Connector will be visible


# Using the Connector within Power BI

Create your ODBC Connection within your windows ODBC Manager - Copy the DSN Name "This is the name of your connection".

DSN is the only mandatory parameter within powerbi along with any username and password when you use the connector.

Please use at your own risk - Works ok for our reporting requirements. - We tested most scenarios... BETA but Works.

# Presto Notes ****

BigInt - Powerbi issues with BigInt -- Fixed on 09/11/2018 release
Decimal - Working Ok - Prefer Double -- Works with Decimal Fields Fixed on 09/11/2018 release
Gateway Support - Checked with Treasure Data ODBC Adaptor - ODBC Connections needs to be under userDSN and systemDSN named the same for the gateway to work properly on the machine where the gateway will be installed.


