This repo is unlikely be updated anymore. Due to IBM [releasing their own ODBC drivers](http://ibm.biz/ibmi-odbc-download), we strongly recommend you use their driver instead. It's far more reliable and supported, can be used on other platforms in .NET, and will work for other PASE software as well. The approach this library took talks to SQL/CLI in the ILE instead, and has stability issues caused by bugs in SQL/CLI.

----

This is a version of the IBM DB2 LUW (Linux/Unix/Windows) ADO.NET provider included with Mono, adapted to work with libdb400. It's quite hacky.

A fresh project file scaffolding was created, as the previous one was very crumbly outside the context of Mono's build system.

## Connecting

A connection string like `"dsn=<DSN HERE>;uid=<YOUR USER HERE>"` - replace the UID with the current user for i, and replace the DSN with the `*LOCAL` entry appropriate. You can find the right `*LOCAL` entry through `WRKRDBDIRE`. No password is required.
