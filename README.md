# Stock Watch

A dashboard that flags which products need attention today — so you don't have to scan every row by hand.

**Live app:** [inventory-urgency.vercel.app](https://inventory-urgency.vercel.app)

## What it does

Given a list of dairy products (name, brand, location, quantity on hand, reorder threshold, expiration date), the app automatically flags a product as urgent if either is true:

- Low stock — quantity is at or below its reorder threshold
- Expiring soon — expiration date is within 14 days of its record date (already past it counts as Expired)

Products are checked automatically as soon as they load — there's no button to click. They render in a single list, with urgent products bordered and tagged with why (Low stock / Expires in Xd / Expired), and everything else tagged "All good". A summary line shows how many products were checked and when, and a stats row breaks down how many need attention versus are fine for now.

## Filtering and sorting

- **Search** by product name
- **Sort** by name or by expiration date
- **Filter chips** narrow the list to a specific reason (Low stock / Expiring soon / Expired)
- **Location filter** narrows the list to a specific location from the dataset

Search, sort, the reason filter, and the location filter all combine — you can use them together.

## Built with

Plain HTML, CSS, and vanilla JavaScript — no framework, no build step.

## Running locally

Just open index.html in a browser. No install required.
