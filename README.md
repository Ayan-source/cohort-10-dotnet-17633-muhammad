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
Database setup and authentication are not implemented yet.

## Frontend setup

Requires Node.js 20.19+ or 22.12+ and npm. The frontend uses React JSX,
Vite, and plain CSS. From the repository root:

```powershell
cd frontend
npm ci
npm run dev
```

Open the local URL printed by Vite (normally `http://localhost:5173`).
The current page is a starter screen; account and task screens are not implemented yet.

Build the production assets with `npm run build`. Use `npm ci` to install
the exact dependency versions recorded in `frontend/package-lock.json`.
