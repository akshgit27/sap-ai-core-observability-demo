# SAP AI Core Observability Demo

One tiny public HTTP service for a live SAP AI Core / SAP AI Launchpad observability demo.

The service image is `docker.io/mendhak/http-https-echo:31`.

It:
- logs HTTP requests to container logs
- echoes request details
- can expose Prometheus metrics at `/metrics`
- can simulate slow responses with `x-set-response-delay-ms`
- can simulate errors with `x-set-response-status-code`

The SAP AI Core serving template is `serving-template.yaml`.
