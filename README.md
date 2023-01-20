# ghls-template

Template repository for [gh-lang-stats](https://github.com/vladaviedov/gh-lang-stats).

## Setup

1. [Use](https://github.com/vladaviedov/ghls-template/generate) this template.
2. Generate a personal access token [here](https://github.com/settings/tokens).
3. Add a your personal access token as a repository secret named `TOKEN` [here](../../settings/secrets/actions) (link only works from README).
4. Pick a template from the [source repo](https://github.com/vladaviedov/gh-lang-stats/tree/master/templates) and copy it to the repository.
5. Rename the file to `template.svg` (or specify with `INPUT_FILE`).
6. Optional (for cron): Uncomment lines 5 and 6 in the [workflow](.github/workflows/generate.yml).

## Usage

Two ways to run it

1. Run it manually from the [Actions](../../actions/workflows/generate.yml) tab.
2. Use cron to run the job automatically (step 6).
	- The default setting is to run it at 00:00 once a day.

The workflow will generate a file `generated.svg` (or specified by `OUTPUT_FILE`).
