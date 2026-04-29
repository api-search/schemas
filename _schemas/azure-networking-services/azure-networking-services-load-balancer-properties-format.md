---
description: Properties of the load balancer.
layout: schema
name: LoadBalancerPropertiesFormat
properties_list:
- description: Collection of backend address pools used by a load balancer.
  name: backendAddressPools
  type: array
- description: Object representing the frontend IPs to be used for the load balancer.
  name: frontendIPConfigurations
  type: array
- description: Defines an external port range for inbound NAT to a single backend port on NICs associated with a load balancer. Inbound NAT rules are created automatically for each NIC associated with the Load Balan
  name: inboundNatPools
  type: array
- description: Collection of inbound NAT Rules used by a load balancer. Defining inbound NAT rules on your load balancer is mutually exclusive with defining an inbound NAT pool. Inbound NAT pools are referenced from
  name: inboundNatRules
  type: array
- description: Object collection representing the load balancing rules Gets the provisioning.
  name: loadBalancingRules
  type: array
- description: The outbound rules.
  name: outboundRules
  type: array
- description: Collection of probe objects used in the load balancer.
  name: probes
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The resource GUID property of the load balancer resource.
  name: resourceGuid
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancer-properties-format-schema.json
slug: azure-networking-services-load-balancer-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-properties-format-schema.json\",\n  \"title\": \"LoadBalancerPropertiesFormat\",\n  \"description\": \"Properties of the load balancer.\",\n  \"properties\": {\n    \"backendAddressPools\": {\n      \"description\": \"Collection of backend address pools used by a load balancer.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/BackendAddressPool\"\n      },\n      \"type\": \"array\"\n    },\n    \"frontendIPConfigurations\": {\n      \"description\": \"Object representing the frontend IPs to be used for the load balancer.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FrontendIPConfiguration\"\n      },\n      \"type\": \"array\"\n    },\n    \"inboundNatPools\": {\n      \"description\": \"Defines an external port range for inbound\
  \ NAT to a single backend port on NICs associated with a load balancer. Inbound NAT rules are created automatically for each NIC associated with the Load Balancer using an external port from this range. Defining an Inbound NAT pool on your Load Balancer is mutually exclusive with defining inbound Nat rules. Inbound NAT pools are referenced from virtual machine scale sets. NICs that are associated with individual virtual machines cannot reference an inbound NAT pool. They have to reference individual inbound NAT rules.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/InboundNatPool\"\n      },\n      \"type\": \"array\"\n    },\n    \"inboundNatRules\": {\n      \"description\": \"Collection of inbound NAT Rules used by a load balancer. Defining inbound NAT rules on your load balancer is mutually exclusive with defining an inbound NAT pool. Inbound NAT pools are referenced from virtual machine scale sets. NICs that are associated with individual virtual machines cannot reference\
  \ an Inbound NAT pool. They have to reference individual inbound NAT rules.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/InboundNatRule\"\n      },\n      \"type\": \"array\"\n    },\n    \"loadBalancingRules\": {\n      \"description\": \"Object collection representing the load balancing rules Gets the provisioning.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/LoadBalancingRule\"\n      },\n      \"type\": \"array\"\n    },\n    \"outboundRules\": {\n      \"description\": \"The outbound rules.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/OutboundRule\"\n      },\n      \"type\": \"array\"\n    },\n    \"probes\": {\n      \"description\": \"Collection of probe objects used in the load balancer.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Probe\"\n      },\n      \"type\": \"array\"\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"\
  Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    },\n    \"resourceGuid\": {\n      \"description\": \"The resource GUID property of the load balancer resource.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancerPropertiesFormat
---
