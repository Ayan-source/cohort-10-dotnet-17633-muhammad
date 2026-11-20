# cohort-10-dotnet-17633-muhammad

Cohort 10 — .NET Fullstack (.NET+ReactJS) assignment for Muhammad Ayan Hussain

## Backend setup

Requires the .NET 10 SDK. Run these commands from the repository root:

```powershell
dotnet restore TaskManager.slnx --locked-mode
dotnet build TaskManager.slnx --no-restore
dotnet run --project backend/TaskManager.Api --launch-profile http
```

Open `http://localhost:5100/api/health`. A running API returns:

```json
{"status":"healthy"}
```

This endpoint checks that the API responds; it does not check a database connection.
Database setup, authentication, and the frontend are not implemented yet.
