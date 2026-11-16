# TubePilot Product Hunt Automation

This repository is the approval-first home for a planned TubePilot Product Hunt workflow.

## Important publishing boundary

The workflow must not publish comments, maker updates, or promotional content to Product Hunt unless Product Hunt has explicitly approved the required API write access and the exact supported publishing operation.

Product Hunt API applications are read-only by default. Do not attempt browser automation, scraping, undocumented endpoints, or reuse of a logged-in browser session to bypass that restriction.

## Current status

- Repository setup: in progress
- Product Hunt API write approval: not yet confirmed
- Automated publishing: disabled
- No API credentials should be committed to this repository

## Before enabling any publishing

1. Obtain written approval from Product Hunt for the required write scope and intended use.
2. Confirm in writing which API mutation supports the intended action on an existing live launch.
3. Confirm whether scheduled recurring maker updates/comments are permitted.
4. Store approved credentials only as GitHub Actions secrets; never commit tokens or secrets.
5. Implement only the documented and explicitly approved API operation.

## Planned secrets (only after approval)

- `PRODUCT_HUNT_CLIENT_ID`
- `PRODUCT_HUNT_CLIENT_SECRET`
- `PRODUCT_HUNT_ACCESS_TOKEN`

No workflow in this repository should publish anything while approval is pending.
