# playground-packer-aws
Packer box for AWS with nginx

## create AWS ec2 instance with packer

apply the same principle when you build the local box with packer.
```
packer build nginx.json
```

## in order to have kitchen test for your ec2 instance do the following

The preferred way to provide credentials to Test Kitchen is to assign the keys to the following environment variables on your workstation.

```
AWS_ACCESS_KEY 
AWS_SECRET_KEY
```

## pre-requisites

configure your own 
```
- VPC
- subnet
- internet gateway
```

or use default

## run the test

```
bundle exec kitchen test
```

