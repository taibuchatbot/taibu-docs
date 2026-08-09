# Connections and keys

**Plug icon → "Connections"** — the systems your AI can reach. Connect a tool once and every skill and routine can use it.

Green means ready, amber means partly set up, grey means not connected.

![The Connections page](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/20-connections.png)

## Three kinds

**API-key tools** (Stripe, HubSpot, QuickBooks, Meta Ads, Google Ads, and locally Merit Aktiva, Montonio, Pipedrive). Press "Connect" and Taibu explains which keys you need, where to get them, and walks you through adding them.

**Live connections** (Notion, Slack, ClickUp, GitHub, Browser). Press "Connect" and Taibu sets it up with you step by step.

**Claude account connectors** (Gmail, Google Drive, Google Calendar). These are switched on in Claude's own connector settings, tied to your account rather than one project. Once connected there, they work everywhere.

The tools on offer differ by language, because the useful accounting and CRM tools differ by market.

"Test" makes one small read-only call to confirm a connection works.

## Keys

**Gear icon → Settings → "Keys"**

Add a key with its name (like STRIPE_SECRET_KEY) and value, then "Add". The eye button reveals a value; the trash removes it. Edits save when you click away or press Enter.

![The Keys tab](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/21-keys.png)

**Never paste an API key into the chat.** Taibu always sends you to this panel instead. Keys are stored per project in a plain file on your disk, so treat that folder like a password file: keep it out of public repositories and shared drives.
