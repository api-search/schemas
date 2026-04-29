---
description: A complex type that contains information about a Resolver configuration for a VPC.
layout: schema
name: ResolverConfig
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
  name: AutodefinedReverse
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-resolver-config-schema.json
slug: amazon-route53-resolver-openapi-resolver-config
source_filename: amazon-route53-resolver-openapi-resolver-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-config-schema.json\",\n  \"title\": \"ResolverConfig\",\n  \"description\": \"A complex type that contains information about a Resolver configuration for a VPC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"ID for the Resolver configuration.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Virtual Private Cloud VPC that you're configuring Resolver for.\"\n        }\n      ]\n    },\n    \"OwnerId\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The owner account ID of the Amazon Virtual Private Cloud VPC.\"\n        }\n      ]\n    },\n    \"AutodefinedReverse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverAutodefinedReverseStatus\"\n        },\n        {\n          \"description\": \"<p> The status of whether or not the Resolver will create autodefined rules for reverse DNS lookups. This is enabled by default. The status can be one of following:</p> <ul> <li> <p> <b>ENABLING:</b> Autodefined rules for reverse DNS lookups are being enabled but are not complete.</p> </li> <li> <p> <b>ENABLED:</b> Autodefined rules for reverse DNS lookups are enabled.</p> </li> <li> <p> <b>DISABLING:</b> Autodefined rules for reverse DNS lookups are being disabled but are not complete.</p> </li> <li> <p> <b>DISABLED:</b> Autodefined rules for reverse DNS lookups are disabled.</p> </li> </ul>\"\n  \
  \      }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-config-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ResolverConfig
---
