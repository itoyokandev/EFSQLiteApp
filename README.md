# .NET����SQLite���p�ɂ���

�Q��URL
* [EF Core �̊T�v](https://docs.microsoft.com/ja-jp/ef/core/get-started/overview/first-app?tabs=netcore-cli)
* [Entity Framework Core �c�[���̃��t�@�����X - Visual Studio �̃p�b�P�[�W �}�l�[�W���[ �R���\�[��](https://docs.microsoft.com/ja-jp/ef/core/cli/powershell)
* 


Nuget�p�b�P�[�W
* Microsoft.EntityFrameworkCore.Sqlite
* Microsoft.EntityFrameworkCore.Tools

EF Core�̊T�v�����Ƃ�DbContext���p���������f�����\������R���e�L�X�g�N���X����уG���e�B�e�B�N���X���`����B

�f�[�^�x�[�X���쐬����
Windows�^�[�~�i���A�v���W�F�N�g�f�B���N�g���ňȉ��̃R�}���h�����s����B

``` .NET CLI
dotnet tool install --global dotnet-ef
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet ef migrations add InitialCreate
dotnet ef database update
```

Program.cs���C������B

���s����
```
Database path: C:\Users\xxx\AppData\Local\blogging.db
Inserting a new blog
Quaring for a blog
Updating the blog and adding a post
Delete the blog
```