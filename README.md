# NetMigrations

Add-Migration InitialCarrierEntities -context <<ContextName>> -OutputDir "Migrations/Read"

Update-database -context <<ContextName>>
  
Remove-Migration -context <<ContextName>>
