# Learn Terraform - HashiCups Provider

This is the companion repo for [Perform CRUD Operations with Providers](https://learn.hashicorp.com/tutorials/terraform/provider-use?in=terraform/providers) tutorial on Learn.


## hashicups
``` shell
curl -Lo terraform-provider-hashicups https://github.com/hashicorp/terraform-provider-hashicups/releases/download/v0.3.1/terraform-provider-hashicups_0.3.1_windows_amd64.zip


mkdir -p $APPDATA/terraform.d/plugins/hashicorp.com/edu/hashicups/0.3.1/windows_amd64

unzip terraform-provider-hashicups -d $APPDATA/terraform.d/plugins/hashicorp.com/edu/hashicups/0.3.1/windows_amd64

icacls "$APPDATA/terraform.d/plugins/hashicorp.com/edu/hashicups/0.3.1/windows_amd64/terraform-provider-hashicups_v0.3.1.exe" /grant USER:RX

icacls "$APPDATA/terraform.d/plugins/hashicorp.com/edu/hashicups/windows_amd64/terraform-provider-hashicups_v0.3.1.exe" /grant USER:RX


curl -X POST localhost:19090/signin -d '{"username":"education", "password":"test123"}'
{"UserID":1,"Username":"education","token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2NTA4NTA1NTQsInVzZXJfaWQiOjEsInVzZXJuYW1lIjoiZWR1Y2F0aW9uIn0.xa5GgtxVGc6AVVCrAMQx-LqaNVpzOTNK2H_QyAc_FsE"}

export HASHICUPS_TOKEN=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2NTA4NTA1NTQsInVzZXJfaWQiOjEsInVzZXJuYW1lIjoiZWR1Y2F0aW9uIn0.xa5GgtxVGc6AVVCrAMQx-LqaNVpzOTNK2H_QyAc_FsE

curl -X POST localhost:19090/signin -d '{"username":"education", "password":"test123"}'
{"UserID":1,"Username":"education","token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2NTA4NTA1NTQsInVzZXJfaWQiOjEsInVzZXJuYW1lIjoiZWR1Y2F0aW9uIn0.xa5GgtxVGc6AVVCrAMQx-LqaNVpzOTNK2H_QyAc_FsE"}
```
