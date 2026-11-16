# Health Savings Bank

A frontend-only administration dashboard prototype for the Health Savings Bank project.

## Frontend scope

This repository currently contains a standalone HTML, CSS and JavaScript frontend. It intentionally does **not** implement a backend, database, authentication, real financial ledger, or payment-provider integration.

### Included screens

- Overview dashboard with summary cards and an illustrative savings activity chart
- Customer directory with search, sample customer creation and customer detail views
- Savings account list and customer balances
- Transaction ledger with search, status filtering, detail views and CSV export
- Medical payment request list
- Example healthcare provider directory
- Reports and account-balance summaries
- Payment integration placeholders for future backend work
- Workspace settings page

### Run locally

You can open `index.html` in a browser, or use the VS Code **Live Server** extension and select **Open with Live Server**.

The frontend loads Bootstrap, Bootstrap Icons, Chart.js and web fonts from CDNs, so an internet connection is needed for those assets.

## Important demo notes

- All customer names, balances, transactions, providers and chart figures are fictional sample data.
- Adding a customer or transaction changes browser memory only. Refreshing the page restores the original sample data.
- CSV exports contain sample data.
- No actual money is stored, transferred, deposited or withdrawn.
- The payment-provider screen is a placeholder only. It does not call MTN MoMo, FNB, eMali, Unayo or any other service.
- Do not enter real customer information or financial details.

## Frontend files

```
index.html
assets/
  css/
    styles.css
  js/
    app.js
```

## Backend handoff

The frontend is intentionally decoupled so the backend developer can later replace the demo data and browser-only actions with ASP.NET Core API calls. Suggested integration points are marked by the screen structure and functions in `assets/js/app.js`.

Keep authentication, authorisation, validation, financial calculations, transaction posting, payment-provider credentials, payment confirmation and reconciliation on the server side.
