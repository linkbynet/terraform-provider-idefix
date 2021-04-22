---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "idefix_ci Resource - terraform-provider-idefix"
subcategory: ""
description: |-
  Manages CI.
---

# idefix_ci (Resource)

Manages CI.

## Example Usage

```terraform
resource "idefix_ci" "example" {
  name        = "myci"
  company_id  = 1234
  project_ids = [1, 2]
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **company_id** (Number) The company ID associated to the CI.
- **id** (String) The ID of this resource.
- **name** (String) The name of this CI.
- **project_ids** (List of Number) The projects associated to the CI.

### Optional

- **comment** (String) Comment.
- **is_owner_lbn** (Boolean) The owner of the CI.
- **outsourcing_name** (String) The Outsourcing level name.
- **service_level_id** (Number) The Level of the service.
- **team** (String) The team in charge.
- **type_id** (Number) The type of the CI.

## Import

Import is supported using the following syntax:

```shell
terraform import idefix_ci.example 1234
```