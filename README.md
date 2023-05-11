See:https://onexlab-io.medium.com/localstack-s3-terraform-9b1554e2add8

### Installation 

## Option 1: Docker-compose 
```
docker-compose up
```



## Option 2: Manual Installation
Install localstack in your environment of choice (ie venv)
```
virtualenv -p python3 venv
pip install localstack
source/venv/bin/activate
localstack launch -d
```

### View service status
View localstack services
```
localstack status services
```

Web browser/ api health check
http://localhost:4566/health

### Stop Localstack
```
docker stop localstack_main
```
Tflocal with Terraform Setup:
https://docs.localstack.cloud/user-guide/integrations/terraform/

https://registry.terraform.io/providers/hashicorp/aws/latest/docs/guides/custom-service-endpoints#localstack
