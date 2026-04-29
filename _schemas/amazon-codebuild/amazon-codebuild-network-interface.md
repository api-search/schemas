---
description: Describes a network interface.
layout: schema
name: NetworkInterface
properties_list:
- description: ''
  name: subnetId
  type: object
- description: ''
  name: networkInterfaceId
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-network-interface-schema.json
slug: amazon-codebuild-network-interface
source_filename: amazon-codebuild-network-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-network-interface-schema.json\",\n  \"title\": \"NetworkInterface\",\n  \"description\": \"Describes a network interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the subnet.\"\n        }\n      ]\n    },\n    \"networkInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the network interface.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-network-interface-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: NetworkInterface
---
