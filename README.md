# SimpleNuget
Steps to create code for a simple nuget package to work through the version naming issues in ADO pipeline builds.

```
SimpleNuget on  master 
❯ ls
total 0
drwxrwxrwx 1 mdb 4.0K Apr 14 08:54 .        
drwxrwxrwx 1 mdb 4.0K Apr 14 08:54 ..       
drwxrwxrwx 1 mdb 4.0K Apr 14 08:54 .git     
-rw-rw-rw- 1 mdb   13 Apr 14 08:54 README.md

SimpleNuget on  master 
❯ mkdir DemoLogger

SimpleNuget on  master 
❯ cd DemoLogger

SimpleNuget/DemoLogger on  master 
❯ dotnet new classlib
The template "Class library" was created successfully.

Processing post-creation actions...
Running 'dotnet restore' on /c/Users/browmik/source/repos/SimpleNuget/DemoLogger/DemoLogger.csproj...
  Restore completed in 333.47 ms for /c/Users/browmik/source/repos/SimpleNuget/DemoLogger/DemoLogger.csproj.

Restore succeeded.
```
Updated the contents of DemoLogger/DemoLogger.csproj with the package info.
Then updated the contents of .gitignore to exclude the bin and obj sub directories.

```
SimpleNuget/DemoLogger on  master [!?] via •NET v2.2.402 
❯ dotnet pack
Microsoft (R) Build Engine version 16.2.32702+c4012a063 for .NET Core
Copyright (C) Microsoft Corporation. All rights reserved.

  Restore completed in 61.69 ms for /c/Users/browmik/source/repos/SimpleNuget/DemoLogger/DemoLogger.csproj.
  DemoLogger -> /c/Users/browmik/source/repos/SimpleNuget/DemoLogger/bin/Debug/netstandard2.0/DemoLogger.dll
  Successfully created package '/c/Users/browmik/source/repos/SimpleNuget/DemoLogger/bin/Debug/DemoLogger.1.0.0.nupkg'.
```