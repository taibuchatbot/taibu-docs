# Apps

An **app** is a small tool Taibu builds for you: a dashboard of your numbers, a report page, a KPI view.

**Grid icon → "Apps"**

## Getting one

Just ask: *"build me an app showing my ad results"* or *"turn my invoices into a dashboard"*. Taibu builds it and adds it to this page automatically.

Two kinds get built:

- **Live** — a small local server, so the data is fresh every time you open it
- **Snapshot** — a single HTML file with the data baked in, safe to send to someone

## Adding one yourself

**"Add app"** takes a name, an address (like http://localhost:8000) or an HTML file, and optionally a start command. The start command runs in the built-in terminal when you open the app, so its server starts by itself.

## If an app is blank

Its server is not running. Press **"Start server"**, or start it yourself, then **"Reload"**.
