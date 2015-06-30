# Introduction #

So you want to use odbc from your Go project? Perhaps you prefer Microsoft's SQL server over alternatives or you need to connect to a third party database? Look no further!

Installing odbc itself is as easy as running `go get code.google.com/p/odbc` but there are some prerequisites you need to have on your OS X system to get started. This page will help you get started.

After following this guide, you should be able to connect to a Microsoft SQL Server from your Go code running on a OS X machine.

## unixODBC ##
You need to install unixODBC, preferably version 2.3.1 or higher because of bugs in the older versions. See [installing unixODBC](InstallingUnixODBCOnOSX.md).


## SQL Driver ##
Besides unixODBC, you'll also need to install the FreeTDS SQL driver.


## Testing your setup ##
After you've installed unixODBC and the FreeTDS driver, it would be wise to test your setup to make sure that everything is working correctly.
See the page on [running the unit tests](RunningTests.md) for more information.

## Get coding! ##
odbc behaves like any other [sql.DB](http://golang.org/pkg/database/sql/) so provided you write your queries in the appropriate SQL dialect existing documentation and tutorials on how to do database connectivity in Go should still apply.