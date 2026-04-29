---
description: <p>Provides authorization for Amazon to bring a specific IP address range to a specific Amazon Web Services account using bring your own IP addresses (BYOIP). </p> <p>For more information, see <a href="https://docs.aws.amazon.com/global-accelerator/latest/dg/using-byoip.html">Bring your own IP addresses (BYOIP)</a> in the <i>Global Accelerator Developer Guide</i>.</p>
layout: schema
name: CidrAuthorizationContext
properties_list:
- description: ''
  name: Message
  type: object
- description: ''
  name: Signature
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-cidr-authorization-context-schema.json
slug: global-accelerator-cidr-authorization-context
source_filename: global-accelerator-cidr-authorization-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-cidr-authorization-context-schema.json\",\n  \"title\": \"CidrAuthorizationContext\",\n  \"description\": \"<p>Provides authorization for Amazon to bring a specific IP address range to a specific Amazon Web Services account using bring your own IP addresses (BYOIP). </p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/using-byoip.html\\\">Bring your own IP addresses (BYOIP)</a> in the <i>Global Accelerator Developer Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The plain-text authorization message for the prefix and account.\"\n        }\n      ]\n\
  \    },\n    \"Signature\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The signed authorization message for the prefix and account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Message\",\n    \"Signature\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-cidr-authorization-context-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CidrAuthorizationContext
---
