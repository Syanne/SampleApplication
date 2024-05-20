# Db Setup

1. Please create an empty database with user, that has an db_owner role. Then replace a ReadWriteDbConnection in Sample.Auth.Api/appsettings.json 
2. Select Sample.Auth.Api (Identity server) as Startup
3. Execure following instructions:
   ```
    Update-Database -Project Sample.Auth.DataAccess.MsSql -Context ConfigurationDbContext
    Update-Database -Project Sample.Auth.DataAccess.MsSql -Context PersistedGrantDbContext
    Update-Database -Project Sample.Auth.DataAccess.MsSql -Context ReadWriteDbContext
   ```

# Run application
Please run both Sample.Auth.Api and Sample.ConsoleApp and follow instructions in Sample.ConsoleApp

You have a pre-set up user. Credentials:
userName: sampleUser@test.com
password: sampleUser@test.com




