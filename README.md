# dagster-offline
Simple offline dagster project for experimenting


## Goals

* dagster init https://docs.dagster.io/api/dg/create-dagster
* use components
* ingest / raw schema
  * 1-2 api calls (fetch some data)
  * maybe use cron?
* transform / silver schema
  * simple data transform
  * eager automation condition
* sensor på ingest assets
* freshness check
* asset check
* abstractions
  * decorators > general asset_checks
  * decorators > timestamp add standard columns

## Later goals
* Machine learning / gold schema
  * ML, random forest
  * model card
  * save model history (revert)
  * Use ML flow