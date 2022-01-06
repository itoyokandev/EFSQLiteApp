# .NETからSQLite利用について

参照URL
* [EF Core の概要](https://docs.microsoft.com/ja-jp/ef/core/get-started/overview/first-app?tabs=netcore-cli)
* [Entity Framework Core ツールのリファレンス - Visual Studio のパッケージ マネージャー コンソール](https://docs.microsoft.com/ja-jp/ef/core/cli/powershell)
* 


Nugetパッケージ
* Microsoft.EntityFrameworkCore.Sqlite
* Microsoft.EntityFrameworkCore.Tools

EF Coreの概要をもとにDbContextを継承したモデルを構成するコンテキストクラスおよびエンティティクラスを定義する。

データベースを作成する
Windowsターミナル、プロジェクトディレクトリで以下のコマンドを実行する。

``` .NET CLI
dotnet tool install --global dotnet-ef
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet ef migrations add InitialCreate
dotnet ef database update
```

Program.csを修正する。

実行結果
```
Database path: C:\Users\xxx\AppData\Local\blogging.db
Inserting a new blog
Quaring for a blog
Updating the blog and adding a post
Delete the blog
```