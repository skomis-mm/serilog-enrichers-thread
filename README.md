# Serilog.Enrichers.Thread [![Build status](https://ci.appveyor.com/api/projects/status/2vgxdy3swg6eaj3f?svg=true)](https://ci.appveyor.com/project/serilog/serilog-enrichers-thread) [![NuGet Version](http://img.shields.io/nuget/v/Serilog.Enrichers.Thread.svg?style=flat)](https://www.nuget.org/packages/Serilog.Enrichers.Thread/)

Enrich Serilog events with properties from the current thread.
 
### Getting started

Install the package from NuGet:

```powershell
Install-Package Serilog.Enrichers.Thread
```

In your logger configuration, apply `Enrich.WithThreadId()`:

```csharp
Log.Logger = new LoggerConfiguration()
    .Enrich.WithThreadId()
    .CreateLogger();
```


Copyright &copy; 2016 Serilog Contributors - Provided under the [Apache License, Version 2.0](http://apache.org/licenses/LICENSE-2.0.html).
