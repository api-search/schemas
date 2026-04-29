---
description: ListComponentProvisionedResourcesInput schema from Amazon Proton API
layout: schema
name: ListComponentProvisionedResourcesInput
properties_list:
- description: ''
  name: componentName
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-component-provisioned-resources-input-schema.json
slug: amazon-proton-list-component-provisioned-resources-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-component-provisioned-resources-input-schema.json\",\n  \"title\": \"ListComponentProvisionedResourcesInput\",\n  \"description\": \"ListComponentProvisionedResourcesInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the component whose provisioned resources you want.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyNextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next provisioned resource in the array of provisioned resources, after the\
  \ list of provisioned resources that was previously requested.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"componentName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-component-provisioned-resources-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListComponentProvisionedResourcesInput
---
