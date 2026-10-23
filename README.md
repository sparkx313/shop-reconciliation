# Daily Sales Reconciliation

A browser-only closeout calculator for a shop's cash, online sales, expenses, and credit entries. It compares a rebuilt manual total with the sales system and can export the result as CSV. No values are sent to a server or saved automatically.

## Use

Open index.html in a modern browser. Enter the business date and all monetary totals, then choose Reconcile day. Download CSV saves the current result to your device.

The calculation assumes the closeout cash count includes the starting float and that listed expenses were paid from that cash:

- Rebuilt cash sales = counted cash - starting float + cash expenses
- Manual total = rebuilt cash sales + online/card sales + patient credit + staff credit
- Variance = manual total - system sales total

Values are rounded to paise before calculation to avoid floating-point currency drift. A positive variance means the manually rebuilt total is higher. Review the assumptions with the shop's accounting process; this tool does not post adjustments or replace a formal accounting system.