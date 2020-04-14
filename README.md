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