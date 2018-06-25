# .NetCodeSnippet
.Net
add-migration "New Entities" -ConfigurationTypeName "MyProjectName.PortalDBOneMigrations.Configuration" -ConnectionString "Server=MSP0VSQLD355\D355; Database=Portal_DB1; Trusted_Connection=True;" -ConnectionProviderName "System.Data.SqlClient" -ProjectName MyProjectName

Update-Database -Verbose -Force -ConnectionString "Server=.; Database=.; Trusted_Connection=True;" -ConnectionProviderName "System.Data.SqlClient"-StartupProjectName MyProjectName.Web  -ProjectName MyProjectName.EntityFramework -ConfigurationTypeName "MyProjectName.PortalDBOneMigrations.Configuration"

