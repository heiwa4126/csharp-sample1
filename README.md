# csharp-sample1

2023-06-30. Windows 11 (x64)

* [.NET を使って作業を開始する | Microsoft Learn](https://learn.microsoft.com/ja-jp/dotnet/core/get-started)
* [.NET ダウンロード (Linux、macOS、Windows)](https://dotnet.microsoft.com/ja-jp/download/dotnet)
* [Chocolatey Software | Microsoft .NET 7.0 SDK 7.0.305](https://community.chocolatey.org/packages/dotnet-7.0-sdk)

管理者権限で

```powershell
choco install dotnet-7.0-sdk
```

作業ディレクトリで

```powershell
dotnet new console -o sample1
cd sample1
dotnet run
```

実行例:

```text
sample1> dotnet run
Hello, World!

sample1> .\bin\Debug\net7.0\sample1.exe
Hello, World!

sample1> dotnet build -c Release
sample1> .\bin\Release\net7.0\sample1.exe
Hello, World!
```

`dotnet new` で出来る `.cs` は BOM付きなので早めに素のUTF-8にしておくこと。

で、

```powershell
dotnet new gitignore
git init
git add --all
git commit -am initial
```

続きは:
[Visual Studio Code を使用して .NET コンソール アプリケーションを作成する - .NET | Microsoft Learn](https://learn.microsoft.com/ja-jp/dotnet/core/tutorials/with-visual-studio-code?pivots=dotnet-7-0)
