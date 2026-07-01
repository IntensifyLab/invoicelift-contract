# Contract Issues Backlog

## Issue: Implement invoice-registry create/approve/assign
**Labels:** `core`, `soroban`
**Description:** Write the smart contract methods to handle the lifecycle of an invoice asset.
**Acceptance Criteria:**
- Only authorized parties can approve/verify an invoice.
- Ownership assignment securely transfers rights to the pool manager.

## Issue: Add concentration and exposure limits in pool-manager
**Labels:** `core`, `finance`
**Description:** Ensure that no single pool is over-exposed to a single buyer or SME to maintain healthy risk distribution.
**Acceptance Criteria:**
- Configurable limits per pool.
- Rejection of financing requests that breach limits.

## Issue: Implement repayment-waterfall principal/fee split
**Labels:** `core`, `finance`
**Description:** Build the logic in `repayment-waterfall` to correctly route incoming funds to principals, protocol fees, and lenders based on predefined precedence.
**Acceptance Criteria:**
- Math precision handles complex splits without rounding errors.
- Disburses funds immediately upon receipt of buyer repayment.

// patch: 2026-06-03T21:05:13.043479

// patch: 2026-06-06T11:41:44.347827

// patch: 2026-06-16T22:07:49.565219

// patch: 2026-07-01T22:07:49.565220
