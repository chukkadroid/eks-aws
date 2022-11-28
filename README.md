# Complete AWS EKS Cluster

Configuration in this directory creates an AWS EKS cluster with a broad mix of various features and settings provided by this module:

- AWS EKS cluster
- Apache tomcat deployment

## Usage

To run this example you need to execute:

```bash
$ terraform init
$ terraform plan
$ terraform apply
$ terraform destroy
```

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.13.1 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 3.72 |
| <a name="requirement_kubernetes"></a> [kubernetes](#requirement\_kubernetes) | >= 2.10 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 3.72 |


## Resources

| Name | Type |
|------|------|
| https://docs.aws.amazon.com/eks/latest/userguide/create-cluster.html | resource |

## Inputs

No inputs.

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_cluster_id"></a> [cluster\_id](#output\_cluster\_id) | The name/id of the EKS cluster. Will block on cluster creation until the cluster is really ready |
| <a name="output_cluster_security_group_id"></a> [cluster\_security\_group\_id](#output\_cluster\_security\_group\_id) | Cluster security group that was created by Amazon EKS for the cluster. Managed node groups use this security group for control-plane-to-data-plane communication. Referred to as 'Cluster security group' in the EKS console |
| <a name="output_cluster_name"></a> [cluster\_role\_name](#output\_cluster\_name) | name of the EKS cluster |
| <a name="output_region"></a> [region\_name](#output\_\_name)region | name of the region |
