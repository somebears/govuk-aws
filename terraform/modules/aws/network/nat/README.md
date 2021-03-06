## Module: aws/network/nat

Create a NAT gateway and associated EIP on each one of the public  
subnets provided.

## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| aws | n/a |

## Modules

No Modules.

## Resources

| Name |
|------|
| [aws_eip](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) |
| [aws_nat_gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| subnet\_ids | List of public subnet IDs where you want to create a NAT Gateway | `list` | n/a | yes |
| subnet\_ids\_length | Length of subnet\_ids variable | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| nat\_gateway\_elastic\_ips\_list | List containing the public IPs associated with the NAT gateways |
| nat\_gateway\_ids | List containing the IDs of the NAT gateways |
| nat\_gateway\_subnets\_ids\_map | Map containing the NAT gateway IDs and the public subnet ID where each one is located |
