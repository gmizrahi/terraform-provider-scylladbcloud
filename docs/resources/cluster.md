---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "scyllacloud_cluster Resource - terraform-provider-scyllacloud"
subcategory: ""
description: |-
  Scylla cluster resource
---

# scyllacloud_cluster (Resource)

Scylla cluster resource

## Example Usage

```terraform
resource "scaffolding_example" "example" {
  configurable_attribute = "some-value"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `broadcast_type` (String) Cluster broadcast type
- `instance_type_id` (Number) ID of the instance type
- `name` (String) Cluster name
- `provider_id` (Number) Cloud provider id
- `provider_region_id` (Number) ID of the cloud provider region
- `replication_factor` (Number) Cluster replication factor
- `user_api_interface` (String) User api interface

### Optional

- `cidr` (String) IPv4 CIDR of the cluster

### Read-Only

- `created_at` (String) Created at
- `dc` (List of Object) Data centers (see [below for nested schema](#nestedatt--dc))
- `dns` (Boolean) Dns
- `encryption_mode` (String) Encryption mode
- `free_tier` (Object) Free tier (see [below for nested schema](#nestedatt--free_tier))
- `grafana_root_url` (String) Grafana root url
- `grafana_url` (String) Grafana url
- `id` (Number) Cluster id
- `max_allowed_cidr_range` (Number) Max allowed cidr range
- `name_on_config_file` (String) Cluster name on config file
- `pricing_model` (Number) Pricing model
- `prom_proxy_enabled` (Boolean) Prom proxy enabled
- `scylla_version` (String) Scylla version
- `scylla_version_id` (Number) Scylla version id
- `status` (String) Cluster status

<a id="nestedatt--dc"></a>
### Nested Schema for `dc`

Read-Only:

- `account_cloud_provider_credential_id` (Number)
- `cidr` (String)
- `client_connection` (List of String)
- `cluster_id` (Number)
- `id` (Number)
- `instance_type_id` (Number)
- `management_network` (String)
- `name` (String)
- `provider_id` (Number)
- `provider_region_id` (Number)
- `replication_factor` (Number)
- `status` (String)


<a id="nestedatt--free_tier"></a>
### Nested Schema for `free_tier`

Read-Only:

- `creation_time` (String)
- `expiration_date` (String)
- `expiration_seconds` (Number)

