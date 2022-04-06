## External-IP Module

This module creates a Google Cloud External IP using the [`google_compute_address`](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_address) resource in the [Google Terraform provider](https://registry.terraform.io/providers/hashicorp/google/latest/docs).

The following information is generated using the
[`terraform-docs`](https://github.com/terraform-docs/terraform-docs)
CLI tool. Use the commands below to re-generate this information during a
release or when you update the variables file. Don't forget to remove the
autogenerated license header after running the tool.

```sh
export VARIABLES_TF_FILE=<PATH_TO_THE_VARIABLES_FILE_FOR_MODULE>
export VARIABLES_MD_FILE=<PATH_TO_THE_VARIABLES_MARKDOWN_FILE>
terraform-docs markdown table --output-file ${VARIABLES_MD_FILE} --output-mode inject ${VARIABLES_TF_FILE}
```

<!-- BEGIN_TF_DOCS -->
## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [google_compute_address.external_ip_address](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_address) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_ip_names"></a> [ip\_names](#input\_ip\_names) | List of names to be used to name the IP addresses | `list(string)` | n/a | yes |
| <a name="input_region"></a> [region](#input\_region) | Region where the IP addresses are to be created in | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_ips"></a> [ips](#output\_ips) | IP information of all the VMs that were created. It is in the form of a map<br>    which has the VM hostname as the key and an object as the value. The object<br>    contains the IP address, tier and region. |
<!-- END_TF_DOCS -->