# ADR 0014 – Error and Retry Strategy

## Status
Accepted

## Decision
The MVP must preserve local draft state on failure and allow safe retries.

## Rules
- never lose the local draft on API failure
- store failure as local state
- show actionable error messages
- allow retry for marketplace creation
- separate validation errors from external API errors

## Example categories
- input/validation error
- template rendering error
- image processing/storage error
- eBay auth error
- eBay API request error

## Why
- reliability over silent failure
- better UX
- easier debugging
