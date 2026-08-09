# Apps

Taibu does not only write about your business. It can **build software for it**. You describe what you want to see, it pulls the data from the tools you have connected, writes the page, and adds it here. No developer, no monthly SaaS fee, no per-seat pricing.

**Grid icon → "Apps"**

![The Apps page](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/22-apps.png)

## Asking for one

The box at the top of the page is the whole interface. Type what you want to see and press **"Build it"**, or Ctrl+Enter. That opens a **new agent** for the job: it plans the app, builds it, and registers it on this page when it is done. You can keep working in another tab meanwhile.

Not sure what to ask for? Watch the box. It types out real examples while you are idle.

Each tile is a **live render of the app itself**, not an icon, so you can tell them apart at a glance. A tile that says **"Not running"** is a live app whose server is stopped: open it and press **"Start server"**.

## One dashboard instead of four browser tabs

Most businesses have the same gap. Ad spend sits in Facebook Ads. More spend sits in Google Ads. Leads arrive through a form on the website. Whether any of it became money sits in the CRM. Nothing joins them up, so nobody can answer the only question that matters: which channel actually pays?

Connect those tools, then ask in one sentence:

> "Build me a live dashboard: ad spend from Facebook and Google, leads from the website funnel, and which of those leads we won in ClickUp. Show cost per lead and return by channel."

![A built app open inside Taibu](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/29-app-open.png)

Look at what that answers. Facebook brings 171 leads at 29 euros each, Google brings 84 at 42. On cost per lead Facebook wins, and most people would move the budget across. But Google closed 10 of its 84 against Facebook's 9 out of 171, so Google returned 5.5 times and Facebook 2.7. The cheaper channel was the worse one, and neither ad platform can tell you that, because neither knows what closed.

## Other things worth building

- **Cash and runway** — bank plus invoices out, so you know the real number
- **Pipeline by stage** — CRM deals, and how long each has been stuck
- **Client report** — one page per client you can send at month end
- **Lead quality by source** — not who sends the most leads, who sends the ones that sign

## Live or snapshot

| Kind | How it works | Use it when |
|---|---|---|
| **Live** | Runs a small local server and re-reads the data each time you open it | It is for you and you want today's numbers |
| **Snapshot** | A single HTML file with the data baked in, no server | You want to send it to a client or your accountant |

A snapshot is one file. Send it and it just opens; the person receiving it needs nothing installed.

## Adding one yourself

Sometimes there is nothing to build: you already have an HTML file, or a server of your own already running. **"Add one manually"** at the bottom of the page takes a name, an address (like http://localhost:8000) or an HTML file, and optionally a start command. The start command runs in the built-in terminal when you open the app, so its server starts by itself.

## If an app is blank

Its server is not running. Press **"Start server"**, or start it yourself, then **"Reload"**. Snapshots never do this, because there is no server to start.

## Where the data goes

An app runs on your computer and reads from the tools you connected. Nothing is uploaded to Taibu. The page is a file in your project that you can open, edit or delete like any other.
