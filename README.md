# NetMigrations

Add-Migration InitialCarrierEntities -context {{ContextName}} -OutputDir "Migrations/Read"

Update-database -context {{ContextName}}
  
Remove-Migration -context {{ContextName}}

Script generation:

Script-Migration -Idempotent -Context {{ContextName}}

appsettings.local.json:
"ConnectionStringName": "User ID={{user}};Password={{pass}};Host=tpm_postgresdatabase;Port=5432;Database={{DbName}};Pooling=true;"
