---
description: UpdateResolverDnssecConfigRequest schema from openapi
layout: schema
name: UpdateResolverDnssecConfigRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Validation
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-resolver-dnssec-config-request-schema.json
slug: amazon-route53-resolver-openapi-update-resolver-dnssec-config-request
source_filename: amazon-route53-resolver-openapi-update-resolver-dnssec-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-dnssec-config-request-schema.json\",\n  \"title\": \"UpdateResolverDnssecConfigRequest\",\n  \"description\": \"UpdateResolverDnssecConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the virtual private cloud (VPC) that you're updating the DNSSEC validation status for.\"\n        }\n      ]\n    },\n    \"Validation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Validation\"\n        },\n        {\n          \"description\": \"The new value that you are specifying for DNSSEC validation for the VPC. The value can\
  \ be <code>ENABLE</code> or <code>DISABLE</code>. Be aware that it can take time for a validation status change to be completed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\",\n    \"Validation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-dnssec-config-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: UpdateResolverDnssecConfigRequest
---
