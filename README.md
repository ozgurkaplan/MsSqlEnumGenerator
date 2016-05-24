# MsSqlEnumGenerator
MsSqlEnumGenerator helps you creates Enums from your tables in MsSql databases.

## Configuration

####App.config
First step is to edit your connection string.
```XML
<connectionStrings>
    <add name="Default" connectionString="Server={ServerIP}; USER ID={UserId}; password={Password}; Database={Database}; PERSIST SECURITY INFO=True;"/>
</connectionStrings>
```

####EnumGenerator.tt
This is place  where you configure bindings. First string is your table name. Second one is the enum text column. Third one is enum value column
```csharp
var enums = new Tuple<string, string, string>[]
{
  //new Tuple<string, string, string>("Table1", "TextColumn", "ValueColumn"),
  //new Tuple<string, string, string>("Table2", "TextColumn", "ValueColumn")
};
```
	
