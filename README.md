# QDT Example Scenarios

[![CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)

This repository contains ready-to-use demo scenarios for testing [QGIS Deployment Toolbelt (QDT)](https://qgis-deployment.github.io/qgis-deployment-toolbelt-cli/) and deploy QGIS profiles.

## Available scenarios

### Example profiles

[`scenario.qdt.yml`](scenarios/scenario.qdt.yml) deploys all the example profiles of the [qdt-examples-qgis-profiles](https://github.com/qgis-deployment/qdt-examples-qgis-profiles) repository (profiles, plugins, shortcuts, splash screen, default profile).

Scenario URL (raw file, ready to be used by QDT):

```text
https://raw.githubusercontent.com/qgis-deployment/qdt-examples-scenarios/refs/heads/main/scenarios/scenario.qdt.yml
```

## Usage

### Prerequisites

- QGIS installed ([download](https://qgis.org/download/))
- QDT installed: see the [installation guide](https://qgis-deployment.github.io/qgis-deployment-toolbelt-cli/usage/installation.html). For example with pipx:

    ```sh
    pipx install qgis-deployment-toolbelt
    ```

### Deploy

Run QDT directly against the remote scenario:

```sh
qdt -s https://raw.githubusercontent.com/qgis-deployment/qdt-examples-scenarios/refs/heads/main/scenarios/scenario.qdt.yml
```

Or clone this repository and use a local scenario:

```sh
git clone https://github.com/qgis-deployment/qdt-examples-scenarios.git
cd qdt-examples-scenarios
qdt -s scenarios/scenario.qdt.yml
```

## Useful links

- [QDT documentation](https://qgis-deployment.github.io/qgis-deployment-toolbelt-cli/)
- [QDT source code](https://github.com/qgis-deployment/qgis-deployment-toolbelt-cli)
- [Scenario reference (jobs and options)](https://qgis-deployment.github.io/qgis-deployment-toolbelt-cli/jobs/)
- [Example QGIS profiles](https://github.com/qgis-deployment/qdt-examples-qgis-profiles)

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).
