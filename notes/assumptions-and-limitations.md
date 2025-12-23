# Assumptions & Limitations

This document outlines the assumptions made during implementation and known limitations of the PFAS checkout solution.

---

## Assumptions

- PFAS applicability could be accurately represented at the product level using Shopify tags
- Shopify Flow and native checkout extensibility were sufficient to enforce compliance logic
- Shipping restrictions were limited to specific U.S. states (CA, NY, ME) at time of implementation
- Customer education at checkout would reduce post-purchase cancellations more effectively than PDP-only warnings

---

## Limitations

- Customers can still add PFAS-restricted products to cart before reaching checkout
- Logic is state-based, not municipality-based
- Checkout warning relies on customers reading and acting on messaging
- Does not prevent users from attempting multiple checkout retries

---

## Tradeoffs & Decisions

- Chose Shopify-native tools over custom code to minimize technical debt
- Accepted minor cart friction in favor of regulatory clarity
- Prioritized early customer communication over silent order blocking

---

## Future Improvements

- Geo-aware PDP messaging based on customer IP
- Expansion to additional regulated regions
- Centralized compliance framework for non-PFAS regulations
