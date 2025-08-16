# dagster-offline
Simple offline dagster project for experimenting


## Goals

* dagster init 
  * https://docs.dagster.io/getting-started/installation 
  * https://docs.dagster.io/api/dg/create-dagster
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

## Installation
* Make sure uv is installed
* Create new project in cwd: `uv init`
* Add packages: `uv add dagster dagster-webserver dagster-dg-cli`
* Verify `dg --version`
* Initialize scaffold in cwd `uvx create-dagster@latest project .`
  * This auto-generates and overwrites existing `README.md`



## Getting started

### Installing dependencies


**Option 1: uv**

Ensure [`uv`](https://docs.astral.sh/uv/) is installed following their [official documentation](https://docs.astral.sh/uv/getting-started/installation/).

Create a virtual environment, and install the required dependencies using _sync_:

```bash
uv sync
```

Then, activate the virtual environment:

| OS | Command |
| --- | --- |
| MacOS | ```source .venv/bin/activate``` |
| Windows | ```.venv\Scripts\activate``` |

**Option 2: pip**

Install the python dependencies with [pip](https://pypi.org/project/pip/):

```bash
python3 -m venv .venv
```

Then active the virtual environment:

| OS | Command |
| --- | --- |
| MacOS | ```source .venv/bin/activate``` |
| Windows | ```.venv\Scripts\activate``` |

Install the required dependencies:

```bash
pip install -e ".[dev]"
```

### Running Dagster

Start the Dagster UI web server:

```bash
dg dev
```

Open http://localhost:3000 in your browser to see the project.

## Learn more

To learn more about this template and Dagster in general:

- [Dagster Documentation](https://docs.dagster.io/)
- [Dagster University](https://courses.dagster.io/)
- [Dagster Slack Community](https://dagster.io/slack)