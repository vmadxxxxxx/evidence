# Evidence [WIP]

Evidence is a service that provides HTTP descriptors for making pre-signed requests and keep track of uploads in progress.

## Docs

You can read about the service capabilities [here](DOCS.md)

## Development

### Requirements

- Docker https://docs.docker.com/compose/install/
- Makefile

### Configuration

You must set the following environment variables in a ``.env`` file:

```
S3_BUCKET='<bucket-name>'
S3_REGION='<region>'
S3_ACCESS_KEY_ID='<access-key-id>'
S3_SECRET_ACCESS_KEY='<secret-access-key>'
```

### Commands

- Boot up development server on http://localhost:7000: ``make up``
- Run tests: ``make-test``
- Show logs: ``make-logs``
- Stop services: ``make-down``
- Clean up: ``make-clean``

## Test

Suites available:

- ``end2end``: Checks that the service API provides the capabilities expected by its consumers.
