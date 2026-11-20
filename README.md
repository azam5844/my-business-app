# AMASS HANDICRAFTS — Quotation & Inventory App

A browser-based quotation and inventory interface for managing product details and preparing customer quotations.

## Features visible in the current app

- Password prompt before opening the interface
- Product entry with item number, description, size, price, and photo
- Product lookup by item number
- Edit product details
- Add products and quantities to a quotation
- Calculate quotation totals
- Print or save the quotation as a PDF through the browser
- Export quotation data as a CSV file for spreadsheet use
- Local browser storage with a Google Apps Script endpoint for cloud data sync

## Run

This project is currently a single-page HTML application.

1. Download or clone the repository.
2. Open `index.html` in a modern browser.
3. Configure and test the cloud sync endpoint in a secure development environment before relying on cloud features.

## Important security notice

The current HTML includes client-side password checking and a cloud-sync endpoint. A password embedded in browser JavaScript is visible to anyone who can inspect the page and is not secure authentication. Do not use this as protection for sensitive business or customer data.

Before public deployment:

- Move authentication and authorization to a trusted server.
- Review access permissions on the connected Google Apps Script and spreadsheet.
- Keep private credentials out of HTML, JavaScript, and public Git history.
- Use HTTPS and validate data on the server.

## Project status

This README describes the current implementation visible in `index.html`. Cloud sync, access control, and data handling should be tested and secured before production use.