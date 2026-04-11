# ADR 0011 – Internal Status Transitions

## Status
Accepted

## Decision
The MVP uses explicit internal workflow states for each draft.

## States
- `draft`
- `classified`
- `needs_attention`
- `ready_for_review`
- `ready_for_marketplace`
- `offer_created`
- `published`
- `blocked`
- `error`

## Transition examples
- upload complete -> `draft`
- first analysis complete -> `classified`
- missing key information -> `needs_attention`
- user confirms/corrects -> `ready_for_review`
- review accepted -> `ready_for_marketplace`
- eBay offer created -> `offer_created`
- later publishing step -> `published`
- unresolved blocker -> `blocked`
- technical failure -> `error`

## Why
- clear UI state
- retry-safe process handling
- easier debugging and persistence
