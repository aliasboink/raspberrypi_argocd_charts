# raspberrypi_argocd_charts
## Manually deployed resources
### Postgresql
For the purpose of using a locally hosted postgresql database the following a [service without selectors](https://kubernetes.io/docs/concepts/services-networking/service/#services-without-selectors) is used.

The resources necessary are present in the `manual/` directory.
- Endpoint
- Service

With the current setup these two are required for the RSS aggregator and Gitea. The namespace in which these are deployed is `postgresql-local`.