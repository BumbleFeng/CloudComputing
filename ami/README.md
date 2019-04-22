# AWS AMI  

## Validate Template  

```
packer validate centos-ami.json
```

## Build AMI  

```
packer build \
    -var 'aws_access_key=REDACTED' \
    -var 'aws_secret_key=REDACTED' \
    -var 'aws_region=us-east-1' \
    -var 'subnet_id=REDACTED' \
    centos-ami.json
```
