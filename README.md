# Fantasy Sales League

[Open the dashboard](https://hnguyen2260.github.io/fantasy-sales-league/)

Eight teams, Tuesday 5 p.m. weekly closes, individual contributions, and fantasy points.

**Refreshes hourly, Monday-Friday, 8 a.m.-5 p.m. Pacific**. The dashboard shows the time of the most recent successful Salesforce refresh. GitHub Pages can take a few minutes to publish each update. If a refresh fails, the last successful dashboard remains available.

Week 1 starts September 23, 2026 and closes Tuesday, September 29 at 5 p.m. Pacific. Each following week starts Tuesday at 5:01 p.m. and closes the next Tuesday at 5 p.m. The full 5:00 minute belongs to the ending week. The eight-week schedule ends November 17. Completed weeks count toward win/loss/tie records; future weeks remain blank.

A Tuesday 5:01 p.m. refresh publishes the rollover. Local Pacific time follows daylight saving changes automatically. Calls and tasks use Salesforce Completed Date/Time. Date-only records that cannot be assigned safely across a Tuesday boundary are held out and flagged for review.

Google Cloud Scheduler triggers a Cloud Run job in athletics-bigquery-sandbox. The job reads Salesforce, recalculates the contest, and publishes this self-contained HTML file. Salesforce credentials and the repository deployment key are stored in Google Secret Manager and are not included in this repository or website.

Scoring controls change the viewer's local display. Scheduled refreshes use the approved league scoring rules.
