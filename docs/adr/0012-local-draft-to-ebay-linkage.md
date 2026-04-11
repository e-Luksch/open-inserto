# ADR 0012 – Local Draft to eBay Linkage

## Status
Accepted

## Decision
A local draft remains the system of record and stores the linkage to eBay objects.

## Required stored linkage
- internal `draft_id`
- marketplace `sku`
- `inventoryItemKey`
- `offerId`
- current local workflow state
- timestamps of creation/update

## Principle
The local draft must remain usable even if eBay offer creation fails or has to be retried.

## Why
- stable recovery path
- decouples local work from external API state
- simplifies edits and retries
