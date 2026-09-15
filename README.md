# puddle.datamade.us

**puddle.datamade.us** is no longer active. The site was a [datasette](https://datasette.io/) instance for Chicago and Illinois data and hosted by DataMade. It was shut down due to overwhelming bot and AI scraper traffic, making hosting costs unsustainable.

You can still download the data that was hosted on puddle via the nightly scrapes from their respective GitHub repositories:

- Chicago City Council
  - [scraper code](https://github.com/datamade/chicago-council-scrapers)
  - [SQLite download](https://github.com/datamade/chicago-council-scrapers/releases/download/nightly/chicago_council.db.zip) (937mb)
- Illinois Campaign Contributions
  - [scraper code](https://github.com/datamade/ilcampaigncash/)
  - [SQLite download](https://github.com/datamade/ilcampaigncash/releases/download/nightly/il_campaign_disclosure.db.zip) (459mb)

---

A [datasette](https://datasette.io/) instance for Chicago and Illinois data. Hosted by DataMade.

Data catalog includes:

- Chicago City Council: https://github.com/datamade/chicago-council-scrapers
- Illinois Campaign Contributions: https://github.com/datamade/ilcampaigncash/
- CMAP Legistar: https://github.com/fgregg/cmap-legistar/

Data is updated on a nightly basis via GitHub Actions.

## Development

### Running locally

Follow the datasette installation documentation here: https://docs.datasette.io/en/stable/installation.html#installation

None of the sqlite databases are saved in this repository. You can download one from https://puddle.datamade.us.

Once you do, follow the datasette instructions to run locally: https://docs.datasette.io/en/stable/getting_started.html#using-datasette-on-your-own-computer

### Deployment

This site is hosted on Google Cloud Run. Here's some useful documentation on how it is set up:

- https://docs.datasette.io/en/stable/publish.html
- https://medium.com/@carstensavage/integrate-workload-identity-federation-with-github-actions-google-cloud-1893306f75c5
