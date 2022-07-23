# Play.Common
Common libraries used by the Play services.

## Create and publish package
```powershell
$version="1.0.6"
$owner="gamemicroservices"
dotnet pack src\Play.Common\ --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/play.common -o ..\packages
```