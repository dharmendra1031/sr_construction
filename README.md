# SR Construction

Frontend-only construction management workspace built with Bootstrap 5.3.

## Purpose

A building-construction company manages projects and sites, purchases material, issues stock to work fronts, bills clients through running-account (RA) bills, and tracks supplier/customer balances. The interface is designed around those workflows rather than generic retail POS screens.

## Screens

| Area | Screens |
| --- | --- |
| Workspace | Overview, Projects, Construction Sites |
| Inventory | Material / Item Master, Opening Stock, Stock Adjustment, Stock Valuation, Site Material Issues |
| Purchase | Supplier Management, Purchase Invoices, Purchase Returns, Purchase Payments, Supplier Outstanding, Purchase History |
| Sales & Billing | Customer Management, Sales Invoices / RA Bills, Credit Notes, Sales History |
| Accounts | Cash Account, Bank Account, Customer Ledger, Supplier Ledger, Day Book, Outstanding Report |

There are 24 navigable screens including Overview, with 20 features from the initial requirements plus Projects, Sites, Material Issues and the Overview.

## Usage

Open `index.html` in a browser. Bootstrap and Bootstrap Icons are loaded from public CDNs, so internet access is needed for those styles and icons.

All screen records are *illustrative construction examples*, not actual company transactions. They exist only in `assets/data.js`. No database, APIs, authentication, payment processing, financial posting or persistent storage have been implemented.

Included frontend interactions:
- Project selection, search, status filters and column sorting
- Client-side pagination, record details, and form validation
- CSV export of currently filtered records
- Responsive sidebar and mobile layouts

The forms intentionally **do not save** records. Real posting, invoice numbering, ledger balances and stock movement logic require a backend.

## Files

- `index.html` — app shell and Bootstrap imports
- `assets/logo.svg` — SR Construction brand artwork
- `assets/app.css` — enterprise styling and responsive layout
- `assets/data.js` — screen definitions and example records
- `assets/app.js` — routing, rendering and frontend interactions

Keep future work minimal: introduce backend services only when required and use numeric auto-increment IDs. Avoid UUID/GUID IDs and duplicate models.
