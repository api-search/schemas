---
description: A complex type that contains information about a configuration for DNSSEC validation.
layout: schema
name: ResolverDnssecConfig
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ValidationStatus
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-resolver-dnssec-config-schema.json
slug: amazon-route53-resolver-openapi-resolver-dnssec-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-dnssec-config-schema.json\",\n  \"title\": \"ResolverDnssecConfig\",\n  \"description\": \"A complex type that contains information about a configuration for DNSSEC validation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID for a configuration for DNSSEC validation.\"\n        }\n      ]\n    },\n    \"OwnerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The owner account ID of the virtual private cloud (VPC) for a configuration for DNSSEC validation.\"\n        }\n      ]\n    },\n    \"ResourceId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the virtual private cloud (VPC) that you're configuring the DNSSEC validation status for.\"\n        }\n      ]\n    },\n    \"ValidationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverDNSSECValidationStatus\"\n        },\n        {\n          \"description\": \"<p>The validation status for a DNSSEC configuration. The status can be one of the following:</p> <ul> <li> <p> <b>ENABLING:</b> DNSSEC validation is being enabled but is not complete.</p> </li> <li> <p> <b>ENABLED:</b> DNSSEC validation is enabled.</p> </li> <li> <p> <b>DISABLING:</b> DNSSEC validation is being disabled but is not complete.</p> </li> <li> <p> <b>DISABLED</b> DNSSEC validation is disabled.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-dnssec-config-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ResolverDnssecConfig
---
