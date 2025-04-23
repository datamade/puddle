# puddle.datamade.us

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