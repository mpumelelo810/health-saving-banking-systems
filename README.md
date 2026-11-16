# Health Savings Bank

Administration interface for the Health Savings Bank application.

## Interface

The interface is built with Tabler Core, Tabler Icons, HTML, CSS and JavaScript.

### Sections
- Overview and savings summary
- Customer directory and customer details
- Savings accounts and balances
- Transaction history with search, status filters and CSV export
- Medical payment requests
- Healthcare provider directory
- Financial reports
- Payment channel integration settings

## Run locally

1. Clone or download this repository.
2. Open the project folder in Visual Studio Code.
3. Open `index.html` with the Live Server extension.

The page loads Tabler Core, Tabler Icons and Chart.js from jsDelivr, so an internet connection is required for those libraries.

## Current application state

The interface currently uses local sample records for layout and interaction testing. Changes made in the browser are temporary and are reset when the page is refreshed. No live customer records, funds or payment services are connected.

## Frontend structure

```
index.html
assets/
  css/
    styles.css
  js/
    app.js
```

## Backend integration

The frontend is separate from the server application. Connect the screens to the ASP.NET Core endpoints as those endpoints become available. Keep authentication, access control, financial calculations, transaction posting, payment-provider credentials, payment verification and reconciliation on the server.
