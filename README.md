## Overview

This is an integration test project for the hello-api project. This uses:
- __Junit 4__: testing framework
- __REST Assured__: Good for integration testing real-running services (think of it as a more programmatic cURL)
- __WireMock__: For the purposes here, registers stubbed responses in a standalone WireMock server run as its own container; this representing stubbing out an external dependent service beyond the domain-under-test or ownership.

### Wut do

#### Local setup

1. Pull down the hello-api project locally (and read it's README)
2. Run the `./local-deps.sh` script in the hello-api project to standup external dependencies
3. In this project, simply run the JUnits. That's it.
4. (Optionally) If running subsequent runs, you may need to re-run `./local-deps.sh` from hello-api if integration tests are taking destructive action agains the seed data

#### CI environment setup

TODO: currently under development!
