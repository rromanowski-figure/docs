---
description: A variation of the Asset Onboarding Service that implements the p8e Scope SDK
---

# p8e CEE API

In this section, you'll learn about a practical implementation of the [p8e-scope-sdk](https://github.com/provenance-io/p8e-scope-sdk), the [p8e-gradle-plugin](https://github.com/provenance-io/p8e-gradle-plugin), and the [metadata-asset-model](https://github.com/provenance-io/metadata-asset-model), which together can be used to register new p8e contract specifications ("smart contracts"), then execute those contracts to store data in the Encrypted Object Store and record assets on the Provenance Blockchain.

We will cover the [API Specification](api-specification/) and walk through the proper execution order:

1. Publishing a new p8e contract,
2. Storing data in p8e, and finally
3. Recording a new asset on the Provenance Blockchain ledger.

### Deploying Locally

To run this service locally, be sure to have [Docker](https://www.docker.com) and [Vault by Hashicorp](https://www.vaultproject.io) installed:

```
brew install docker
```

```
brew tap hashicorp/tap
brew install hashicorp/tap/vault
```

once installed, all you need to do is run the included docker setup script

```
./dc.sh up
```

and run the service - either via an Intellij run configuration or via the command line with the following command:

```
./gradlew bootRun
```

### API Key for Test or Production Environments

Coming soon!