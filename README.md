# Bulk Equipment Assignment — Interactive Demo

A standalone interactive simulation demonstrating a browser-based laboratory workflow automation tool developed by **Jonathan Shuhendler**.

**[Try the live demo](https://jshuhendler.github.io/bulk-equipment-assignment-demo/)** 

## Problem

Calibration technicians often need to assign the same balance, hygrometer, and reference weight set to numerous pipettes within a service order. Doing it individually is repetitive and error-prone.

## Solution

The real automation runs in an authenticated Qualer browser session: it identifies selected service-order items, looks up calibration instruments by exact serial number, checks existing assignments, submits missing assignments, and verifies changes.

This GitHub Pages demo **simulates** those steps using fictional instruments and an in-memory catalog. It makes no network calls to Qualer and requires no credentials.

## Try it

1. Select a few sample pipettes.
2. Leave the fictional equipment serial numbers as provided.
3. Click **Assign missing equipment** and watch the verification log.
4. Run it again to see that no duplicate assignments are created.
5. Click **Reset demo** to start over.

## Technical highlights

- Vanilla HTML, CSS and JavaScript (no framework or backend)
- Exact serial-to-equipment-ID lookup against a fictional catalog
- Idempotent assignment logic and post-assignment verification simulation
- Per-pipette progress and status reporting
- Responsive dark UI
- All demo data remains in the browser; no external requests

## Privacy and scope

This is a portfolio demonstration, not the production script. It contains no real client information, Qualer credentials, private API endpoints, or operational access to an authenticated organization.

Developed by [Jonathan Shuhendler](https://github.com/jshuhendler). Not affiliated with Qualer.
