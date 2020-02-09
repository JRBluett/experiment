Install:
    FROM: Ubuntu 18.0.4 LTS
    VSCode
    dotnet-sdk
    Node.js
    npm
    C# VSCode extension

.gitignore
https://www.gitignore.io/

Commands:
    dotnet new mstest -n mainTest
    dotnet new classlib -n corelib
    dotnet new angular -n mainAngular
    dotnet new console -n main
    dotnet new sln -n experiment

    dotnet sln add ./corelib/corelib.csproj 
    dotnet sln add ./main/main.csproj 
    dotnet sln add ./mainAngular/mainAngular.csproj 
    dotnet sln add ./mainTest/mainTest.csproj 

    dotnet add ./main/main.csproj reference ./corelib/corelib.csproj 
    dotnet add ./mainAngular/mainAngular.csproj reference ./corelib/corelib.csproj 
    dotnet add ./mainTest/mainTest.csproj reference ./main/main.csproj 
