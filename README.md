# grafana-cfn-deployment
This is a complete Grafana deployment in a single Cloudformation template.
It runs Grafana on a high availabilty setup and has two environment options: developement and production. 
It was written as an excercise on Cloudformation, but I believe it can be used in real world scenarios.

### Parameters

| Parameter Name | Description |
| ------ | ------ |
| Type of deployment | Choose between dev and prod. Differences on EC2 and RDS families and sizes.|
| User IP | Your IP on CIDR format. This applies only to port 22, so use your own IP. |
| UserKeyPair | A keypair to allow ssh connection. |
| DatabasePassword | The database master password. |