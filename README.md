# Rancher catalog: Sends AWS information to prometheus

Sends AWS information to a Prometheus gateway

## Parameters

### AWS_ACCESS_KEY_ID
AWS access key for API calls

### AWS_SECRET_ACCESS_KEY
AWS secret key for API calls

### AWS_REGION_NAME
AWS region (default: eu-west-1)

### JOB_SCHEDULED
Jobber scheduled time (default: `0 */5 * * * *`)

## Security concern
The script only needs read-only access to EC2 component.

We strongly advice you create a dedicated user with dedicated
API keys per container (in case you want to monitor multiple Regions).
