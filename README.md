This is a version of the IBM DB2 LUW (Linux/Unix/Windows) ADO.NET provider included with Mono, adapted to work with libdb400. It's quite hacky.

A fresh project file scaffolding was created, as the previous one was very crumbly outside the context of Mono's build system.

## Connecting

A connection string like `"dsn=<DSN HERE>;uid=<YOUR USER HERE>"` - replace the UID with the current user for i, and replace the DSN with the `*LOCAL` entry appropriate. You can find the right `*LOCAL` entry through `WRKRDBDIRE`. No password is required.