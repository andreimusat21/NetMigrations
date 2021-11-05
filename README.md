# NetMigrations

Add-Migration InitialCarrierEntities -context {{ContextName}} -OutputDir "Migrations/Read"

Update-database -context {{ContextName}}
  
Remove-Migration -context {{ContextName}}

Script generation
Script-Migration -Idempotent -Context {{ContextName}}
