Test Plan – Sunshine Coffee

1. Objective

Verify that core shopping flows on Sunshine Coffee (product browsing, product
detail, cart, checkout) function correctly across browsers and devices, and that
the public /products API behaves correctly and predictably.

2. Scope

In scope

Product listing page
Product detail page
Cart (add, remove)
Checkout form and submission
/products and /products/:id API endpoints
Responsive behavior (desktop, tablet, mobile widths)
Cross-browser: Chromium, Firefox, WebKit


3. Test Approach

Exploratory testing first, to map flows and surface obvious issues before formal cases are written.
Manual functional testing against written test cases, covering happy paths and edge cases (empty cart, invalid checkout input, non-existent product IDs).
Automated regression for the highest-value, most stable flows using Playwright (UI) and Playwright's API testing for the backend.
Cross-browser/responsive checks run through Playwright's multi-project config.



4. Environment


Browsers: Chromium, Firefox, WebKit (via Playwright)
Viewports: Desktop (1280x720), Mobile 


5. Entry / Exit Criteria

Entry: App is reachable at the live URL and API returns a 200 on /products.

Exit: All planned manual test cases executed and logged; 