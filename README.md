# my-calculator-poc.github.io
The meta repo organize the operations for the POC

## Goals

Design a mobile solution with the following Design:

| FRONT-END |     | BACKEND (First Layer)  |     | BACKEND (Second Layer) |   |
|-----------|-----|------------------------|-----|------------------------|---|
| My Client | SCC | My Calculator API      | SCC | My Sum API             |   |
|           | SCC | Another Calculator API | SCC | My Multiply API        |   |

**Organize contracts by Domain**

The POC includes 2 repositories to store contracts from multiple domains in the Calculator Universe

- https://github.com/my-calculator-poc/my-calculator-contracts-center-domain1
- https://github.com/my-calculator-poc/my-calculator-contracts-center-domain2

**Integration Tests**

In a Integration Tests, it is possible to use with the help of **StubRunnerRule** (Pending Test) contracts from multiple domains, the usage of **@AutoConfigureStubRunner** is limited to only one Git repo:
https://cloud.spring.io/spring-cloud-static/Greenwich.RELEASE/multi/multi__spring_cloud_contract_stub_runner.html

To use the contracts for a mobile consumer, it is possible to use a Docker image or Docker compose:
https://cloud.spring.io/spring-cloud-contract/spring-cloud-contract.html#stubrunner-docker

## CI

- My Calculator API [![Build Status](https://travis-ci.org/my-calculator-poc/My-Calculator-API.svg?branch=master)](https://travis-ci.org/my-calculator-poc/My-Calculator-API)
- My Sum API [![Build Status](https://travis-ci.org/my-calculator-poc/My-Sum-API.svg?branch=master)](https://travis-ci.org/my-calculator-poc/My-Sum-API)
- My Multiply API

## References:

- https://cloud-samples.spring.io/spring-cloud-contract-samples/workshops.html
- https://www.oreilly.com/library/view/hands-on-guide-to/9780135598436/
- https://cloud.spring.io/spring-cloud-contract/spring-cloud-contract.html
- https://cloud.spring.io/spring-cloud-static/Greenwich.RELEASE/multi/multi__spring_cloud_contract.html
- https://cloud.spring.io/spring-cloud-contract/spring-cloud-contract-maven-plugin/complex.html
