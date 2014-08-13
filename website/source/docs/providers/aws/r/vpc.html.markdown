---
layout: "aws"
page_title: "AWS: aws_vpc"
sidebar_current: "docs-aws-resource-vpc"
---

# aws\_vpc

Provides an VPC resource.

## Example Usage

```
resource "aws_vpc" "main" {
    cidr_block = "10.0.0.0/16"
}
```

## Argument Reference

The following arguments are supported:

* `cidr_block` - (Required) The CIDR block for the VPC.
* `enable_dns_support` - (Optional) A boolean flag to enable/disable DNS support in the VPC. Defaults true.
* `enable_dns_hostnames` - (Optional) A boolean flag to enable/disable DNS hostnames in the VPC. Defaults false.

## Attributes Reference

The following attributes are exported:

* `id` - The ID of the VPC
* `cidr_block` - The CIDR block of the VPC
* `enable_dns_support` - Whether or not the VPC has DNS support
* `enable_dns_hostnames` - Whether or not the VPC has DNS hostname support

