---
description: Configuration of the firewall behavior provided by DNS Firewall for a single VPC from Amazon Virtual Private Cloud (Amazon VPC).
layout: schema
name: FirewallConfig
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: FirewallFailOpen
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-firewall-config-schema.json
slug: amazon-route53-resolver-openapi-firewall-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-config-schema.json\",\n  \"title\": \"FirewallConfig\",\n  \"description\": \"Configuration of the firewall behavior provided by DNS Firewall for a single VPC from Amazon Virtual Private Cloud (Amazon VPC). \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the firewall configuration.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the VPC that this firewall configuration applies to.\"\n        }\n      ]\n    },\n    \"OwnerId\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the owner of the VPC that this firewall configuration applies to.\"\n        }\n      ]\n    },\n    \"FirewallFailOpen\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallFailOpenStatus\"\n        },\n        {\n          \"description\": \"<p>Determines how DNS Firewall operates during failures, for example when all traffic that is sent to DNS Firewall fails to receive a reply. </p> <ul> <li> <p>By default, fail open is disabled, which means the failure mode is closed. This approach favors security over availability. DNS Firewall returns a failure error when it is unable to properly evaluate a query. </p> </li> <li> <p>If you enable this option, the failure mode is open. This approach favors availability over security. DNS Firewall allows queries to proceed if it is unable to properly\
  \ evaluate them. </p> </li> </ul> <p>This behavior is only enforced for VPCs that have at least one DNS Firewall rule group association. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-config-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: FirewallConfig
---
