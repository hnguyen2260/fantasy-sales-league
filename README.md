# Fantasy Sales League

[Open the dashboard](https://hnguyen2260.github.io/fantasy-sales-league/)

Eight teams, Wednesday-to-Wednesday matchups, individual contributions, and fantasy points.

**Refreshes hourly, Monday-Friday, 8 a.m.-5 p.m. Pacific**. The dashboard shows the time of the most recent successful Salesforce refresh. GitHub Pages can take a few minutes to publish each update. If a refresh fails, the last successful dashboard remains available.

Week 1 is September 23–30, 2026. Each Wednesday at midnight Pacific starts the next week. The eight-week schedule ends November 18. Completed weeks count toward win/loss/tie records; future weeks remain blank.

Google Cloud Scheduler triggers a Cloud Run job in athletics-bigquery-sandbox. The job reads Salesforce, recalculates the contest, and publishes this self-contained HTML file. Salesforce credentials and the repository deployment key are stored in Google Secret Manager and are not included in this repository or website.

Scoring controls change the viewer's local display. Scheduled refreshes use the approved league scoring rules.
