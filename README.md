# Al Hasan Engineering Works: Website & Boiler ERP Demo

A clickable proposal demo for **M/S Al Hasan Engineering Works**, Chattogram. It shows two things in one page: a public company website and a Boiler ERP for running the business behind it.

**Live demo:** https://asifur-rahman-ai.github.io/alhasan

> ⚠️ All customers, boilers, leads, invoices and figures in the ERP are **sample data** for demonstration. Nothing is saved, and the page resets on reload.

---

## What's inside

Use the **Website / Boiler ERP** switch in the top bar to move between the two demos.

### 1. Company website

- **Hero with official listing plate:** shows the firm's listing as Boiler Repairing Institution (serial no. 43) with the Office of the Chief Inspector of Boilers, Bangladesh. It links to the source page for verification and is not presented as a government endorsement.
- **Ten services** in three groups: Boiler, Water & cooling, Industrial.
- **Regular dosing programme:** a 7-step cycle (Survey → Sample → Analyse → Dose → Monitor → Report → Adjust).
- **Group companies:** Al Hasan Engineering Works with its sister concerns, Hoque Engineering and the water treatment & LPG team.
- **Six-step job process** and a **products & spare parts** list with "Request price" instead of a checkout.
- **Quotation request form** with validation (required fields, 11-digit mobile number, consent).
- **Three locations:** Halishahar office, MEZ office (Mirsarai), Pahartali workshop, each with Google Maps and call links.
- **Mobile quick-contact bar** for Call, WhatsApp and Get quote.

### 2. Boiler ERP

| Module | What it shows |
|---|---|
| Dashboard | Jobs today, open leads, pending quotations, receivables, low stock, upcoming due dates, sales vs expense chart, pipeline |
| Leads & CRM | Kanban pipeline: New lead → Contacted → Site visit → Quotation → Work order → Completed |
| Boiler register | One profile per boiler with registration no., descaling and inspection dates, service history |
| Reminders | Alerts at 90, 60, 30, 15, 7 and 1 day before descaling, inspection renewal and payment due dates |
| Quotations | Line-item builder with discount, VAT, transport, live totals and a printable preview |
| Inventory | Parts, chemicals and water-treatment stock with category filter, search and minimum-stock alerts |
| Service reports | Sample boiler descaling report with readings, safety checklist and signature blocks |
| Marketing | Ad spend, leads, cost per lead and return by campaign and source |
| Roadmap | Phase 1–3 delivery plan |
| My boilers | Customer portal: boilers, invoices, documents and service requests |

**Role-based menus:** switch "Viewing as" between Managing Director, Sales Executive, Engineer / Technician, Storekeeper and Customer (portal). Each role sees only its own modules.

---

## Try the end-to-end flow

1. On the **Website** tab, fill in and submit the **Request a quotation** form.
2. Click **See it arrive in the ERP**, or switch to the **Boiler ERP** tab.
3. Open **Leads & CRM**. Your enquiry is in **New lead**, highlighted, with a "new" badge in the menu.
4. Move it through the pipeline, then build a quotation for it in **Quotations**.

You can also switch the role to **Customer (portal)**, send a service request, then switch back to **Managing Director** to see it in the CRM.

---

## Tech

- A single self-contained `index.html`: HTML, CSS and vanilla JavaScript
- No framework, no build step, no backend, no dependencies
- Google Fonts: Barlow, Barlow Condensed and Hind Siliguri (for Bangla text)
- Responsive down to mobile, with safe-area support for notched phones
- Automatic light and dark theme from the system setting
- Keyboard accessible: focus styles, ARIA labels, Escape to close the preview
- All dates are calculated from today, so reminders and due dates always look current

---

## Run locally

```bash
git clone https://github.com/asifur-rahman-ai/alhasan.git
cd alhasan
```

Then open `index.html` in a browser. Or serve it:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy on GitHub Pages

1. Push `index.html` to the `main` branch.
2. Go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**, then `main` and `/ (root)`.
4. The site goes live at `https://<username>.github.io/<repo>/`.

---

## Project structure

```
alhasan/
├── index.html   # website + ERP demo (markup, styles, script)
└── README.md
```

---

## Roadmap for the full system

| Phase | Scope |
|---|---|
| **Phase 1** (in this demo) | Customer & boiler register, automatic reminders, quotation / invoice / challan, inventory & low-stock alerts, website enquiry to CRM |
| **Phase 2** | Projects & work orders, descaling & inspection reports, accounts with cash & bank book, purchase & suppliers, sales reports |
| **Phase 3** | Customer portal, WhatsApp & SMS automation, employee & technician management, chemical & efficiency calculators, Android app |

In the demo, actions such as sending WhatsApp reminders, assigning jobs, raising purchase requests and downloading PDFs only show a confirmation message. They become real integrations in the full build.

---

## Author

Prepared by **Md. Asifur Rahman** as a proposal for M/S Al Hasan Engineering Works.

Company names, addresses and phone numbers belong to M/S Al Hasan Engineering Works and are used with reference to this proposal only.
