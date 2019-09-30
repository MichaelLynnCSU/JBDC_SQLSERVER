# JBDC_SQLSERVER


# POM

https://mvnrepository.com/artifact/com.microsoft.sqlserver/mssql-jdbc/7.0.0.jre8


# Changing the SQL Server Default Ports

Procedure

From the Start menu, choose All Programs | Microsoft SQL Server 2012 | Configuration Tools | SQL Server Configuration Manager.

Expand the SQL Server 2012 Network Configuration node and select Protocols for the SQL Server instance to be configured.

In the right pane, right-click the protocol name TCP/IP and choose Properties.

In the TCP/IP Properties dialog box, select the IP Addresses tab

Except for the IP addresses under IPAll, clear the values for both the TCP Dynamic Ports and TCP Port for each IP addres

In the IPAll section for each instance, type in a new port for SQL Server 2012 requests and communications. 

Restart the SQL Server Services



# Connect with database which is using windows authentication
 
Procedure
 
DriverManager.getConnection("jdbc:sqlserver://localhost:<defaultport>;integratedSecurity=true;");
  
# Download the JDBC Driver
 
https://www.microsoft.com/en-us/download/details.aspx?id=11774
 
unzip the file and go to sqljdbc_version\fra\auth\x86 or \x64
 
copy the sqljdbc_auth.dll to C:\Program Files\Java\jre_Version\bin
 
restart
 
 
 
