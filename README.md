# Stock Watch

A dashboard that flags which products need attention today — so you don't have to scan every row by hand.

**Live app:** [inventory-urgency.vercel.app](https://inventory-urgency.vercel.app)

## What it does

Given a list of dairy products (name, quantity on hand, reorder threshold, expiration date), the app flags a product as urgent if either is true:

- Low stock — quantity is at or below its reorder threshold
- Expiring soon — expiration date is within the next 14 days

Click Check Urgency to run the check. Results split into two columns:

- Needs Attention Today — flagged products, with chips showing why (Low stock / Expires in Xd / Expired)
- Fine For Now — everything else

A summary line shows how many products were checked and when.

## Built with

Plain HTML, CSS, and vanilla JavaScript — no framework, no build step.

## Running locally

Just open index.html in a browser. No install required.
