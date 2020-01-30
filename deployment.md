# Deployment

This section will be split into two sections; deploying locally for development and deploying to AWS for production.

## Development

Currently development environments are lacking.

Each component will eventually have a `./scripts/run_local` script for bringing up a local development environment - likely via docker-compose.

The master server has a separate docker-compose file that also attempts to link all these separate components into a single stack although this has not been tested lately.

## Production

Deployment to AWS is managed via AWS-CDK stacks written in Python.

- [infrastructure](https://github.com/quakeservices/infrastructure)
- [master](https://github.com/quakeservices/master_deploy)
- [web-frontend](https://github.com/quakeservices/web-frontend_deploy)
- [web-backend](https://github.com/quakeservices/web-backend_deploy)
