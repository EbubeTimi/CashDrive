# CashDrive Codex Guide

This repository contains two standalone web pages:

- `cashdriveintake.html`
- `cashdrivepostinglog.html`

They connect to Google Apps Script and Google Drive workflows used for creator intake and posting operations.

## Working rules

- Read both HTML files and inspect Git status before changing a workflow.
- Preserve the existing operational data flow unless the requested change explicitly replaces it.
- Never add, request, transmit, or store Gmail, Instagram, TikTok, or other account passwords.
- The existing password fields and password submission logic are legacy security debt. Do not test them with real credentials or reproduce that pattern in new work. Plan their removal as a dedicated change before the intake is used further.
- Do not expose Apps Script URLs, access keys, personal data, Drive contents, or admin credentials.
- Do not change a live Apps Script, Drive folder, production data, deployment, or GitHub branch without Smith's explicit approval.

## Validation

There is no automated test suite yet. For changes, validate the page locally, check its browser behavior, and document any live integration that could not be safely tested.
