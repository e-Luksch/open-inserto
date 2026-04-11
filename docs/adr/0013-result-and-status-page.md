# ADR 0013 – Result and Status Page

## Status
Accepted

## Decision
After draft creation or eBay offer creation, the app shows a simple status/result page.

## MVP contents
- draft title
- internal draft id
- current workflow status
- whether review is still needed
- eBay inventory item key (if available)
- eBay offer id (if available)
- last action result
- next recommended action

## Why
- keeps the app understandable
- avoids hidden background state
- makes manual review easy
