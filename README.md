# cloud-run-compose-demo

A demo of Google Cloud Run's new Docker Compose feature, in private preview.

https://cloud.google.com/blog/products/serverless/cloud-run-and-docker-collaboration

## Deploy

To deploy this, run the following command: (make sure you're signed up for the technical preview!)

```bash
gcloud alpha run compose up
```

## Access your Cloud Run service

The resulting Cloud Run service has authentication enabled by default. You can run a proxy to access the service:

```bash
gcloud run services proxy cloud-run-compose-demo
```

Alternatively, you can disable authentication via the Google Cloud Run console.
