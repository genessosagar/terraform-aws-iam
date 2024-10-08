# Individual IAM assumable role example

Configuration in this directory creates a single IAM role which can be assumed by trusted resources using OpenID Connect Federated Users.

# Usage

To run this example you need to execute:

```bash
$ terraform init
$ terraform plan
$ terraform apply
```

Run `terraform destroy` when you don't need these resources.

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 4.0 |

## Providers

No providers.

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_iam_assumable_role_admin"></a> [iam\_assumable\_role\_admin](#module\_iam\_assumable\_role\_admin) | ../../modules/iam-assumable-role-with-oidc | n/a |
| <a name="module_iam_assumable_role_inline_policy"></a> [iam\_assumable\_role\_inline\_policy](#module\_iam\_assumable\_role\_inline\_policy) | ../../modules/iam-assumable-role-with-oidc | n/a |
| <a name="module_iam_assumable_role_provider_trust_policy_conditions"></a> [iam\_assumable\_role\_provider\_trust\_policy\_conditions](#module\_iam\_assumable\_role\_provider\_trust\_policy\_conditions) | ../../modules/iam-assumable-role-with-oidc | n/a |
| <a name="module_iam_assumable_role_self_assume"></a> [iam\_assumable\_role\_self\_assume](#module\_iam\_assumable\_role\_self\_assume) | ../../modules/iam-assumable-role-with-oidc | n/a |

## Resources

No resources.

## Inputs

No inputs.

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_iam_role_arn"></a> [iam\_role\_arn](#output\_iam\_role\_arn) | ARN of IAM role |
| <a name="output_iam_role_name"></a> [iam\_role\_name](#output\_iam\_role\_name) | Name of IAM role |
| <a name="output_iam_role_path"></a> [iam\_role\_path](#output\_iam\_role\_path) | Path of IAM role |
| <a name="output_iam_role_unique_id"></a> [iam\_role\_unique\_id](#output\_iam\_role\_unique\_id) | Unique ID of IAM role |
<!-- END_TF_DOCS -->
