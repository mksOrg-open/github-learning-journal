
Create your app

```
dotnet new webapp -o MentalHealth --no-https -f net6.0
```


```
dotnet add <PROJECT> package <PACKAGE_NAME> [options]
```


Solution:
https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-with-dotnet-test


```
dotnet new sln -o unit-testing-using-dotnet-test
```

```
dotnet new classlib -o PrimeService
```

```c#
using System;

namespace Prime.Services
{
    public class PrimeService
    {
        public bool IsPrime(int candidate)
        {
            throw new NotImplementedException("Not implemented.");
        }
    }
}
```

```sh
dotnet sln add ./PrimeService/PrimeService.csproj
```

```sh
dotnet new xunit -o PrimeService.Tests 
```

Add the `PrimeService` class library as a dependency to the _PrimeService.Tests_ project:

```sh
dotnet add ./PrimeService.Tests/PrimeService.Tests.csproj reference  ./PrimeService/PrimeService.csproj
```

### Commands to create the solution
```sh

dotnet new sln -o unit-testing-using-dotnet-test
cd unit-testing-using-dotnet-test
dotnet new classlib -o PrimeService
ren .\PrimeService\Class1.cs PrimeService.cs
dotnet sln add ./PrimeService/PrimeService.csproj
dotnet new xunit -o PrimeService.Tests
dotnet add ./PrimeService.Tests/PrimeService.Tests.csproj reference ./PrimeService/PrimeService.csproj
dotnet sln add ./PrimeService.Tests/PrimeService.Tests.csproj

```
