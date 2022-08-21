# Play.Common
Common libraries used by the Play services.

## Create and publish package
```powershell
$version="1.0.6"
$owner="gamemicroservices"
$gh_pat="[PAT HERE]"
dotnet pack src\Play.Common\ --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/play.common -o ..\packages

dotnet nuget push ..\packages\Play.Common.$version.nupkg --api-key $gh_pat --source "github"
```