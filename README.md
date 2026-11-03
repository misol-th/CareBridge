# CareBridge — demo prototype

CareBridge is a front-end prototype for monitoring medical inventory and identifying possible stock shortages before the next expected delivery.

## Run locally
1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. The demo starts with sample inventory data. Add, edit, or delete items to test it.

## Features
- Inventory dashboard with sample data.
- Add, edit, search, and delete medicines and supplies.
- Estimate days of stock remaining from current quantity and average daily use.
- Early warnings when stock may run out before the expected delivery.
- Manual emergency/event log.
- Simple increased-demand scenario calculator.
- Export demo data as JSON.
- Responsive layout for desktop and mobile.
- Browser LocalStorage persistence.

## Publish with GitHub Pages
1. Create a GitHub repository, for example `carebridge-prototype`.
2. Upload `index.html` and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for the Pages URL to appear.

## Important limitations
- This is an educational/demo prototype, not a production healthcare system.
- The current version uses transparent rule-based calculations, not a trained AI model.
- Emergency events are entered manually; no live outbreak or emergency alert feed is connected.
- Sample data is fictional. Do not enter patient-identifiable or confidential hospital information.
- It does not provide clinical advice, treatment recommendations, or automatic purchasing.
- Real deployment would require validation with healthcare professionals, security review, access controls, reliable data integrations, and local regulatory assessment.

## Calculation
Estimated days remaining = current stock / average daily usage.

A warning is shown if estimated days remaining are less than the expected delivery lead time. An additional "attention" status is shown when the estimated remaining days are within three days after the expected delivery time. This is a simple planning indicator and should be checked by responsible staff.
