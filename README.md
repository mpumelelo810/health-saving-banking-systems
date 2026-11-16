# Health Savings Bank

Frontend interface for the Health Savings Bank application.

## Portals

- `index.html` — administration portal
- `customer.html` — customer/member portal
- `customer-login.html` — customer sign-in preview

## Administration portal

- Overview and savings summary
- Customer directory and customer details
- Savings accounts and balances
- Transaction history with search, status filters and CSV export
- Medical payment requests
- Healthcare provider directory
- Financial reports
- Payment channel integration settings

## Customer portal

- Member dashboard and available savings balance
- Savings account details
- Sample contribution flow
- Transaction history and CSV export
- Medical payment request form and request history
- Customer profile view and sample profile editing
- Sign-in page preview

## Run locally

1. Clone or download this repository.
2. Open the project folder in Visual Studio Community using **File → Open → Folder**.
3. Open `index.html` to view the administration portal, or `customer.html` to view the customer portal.
4. Use **File → View in Browser**, or open the HTML file from File Explorer.

The pages load Tabler Core, Tabler Icons and (on the administration portal) Chart.js from CDNs, so an internet connection is required for those libraries.

## Current application state

The portals currently use fictional sample records for interface and interaction testing. Changes made in the browser are temporary and reset when the page is refreshed. The sign-in screen is not connected to authentication. No real customer records, funds or payment services are connected.

## Frontend structure

```
index.html
customer.html
customer-login.html
assets/
  css/
    styles.css
    customer.css
  js/
    app.js
    customer.js
```

## Backend integration

The frontend is separate from the server application. Connect the screens to ASP.NET Core endpoints as those endpoints become available. Keep authentication, access control, financial calculations, transaction posting, payment-provider credentials, payment verification and reconciliation on the server.
