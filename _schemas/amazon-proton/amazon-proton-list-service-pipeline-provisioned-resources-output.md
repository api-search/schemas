---
description: ListServicePipelineProvisionedResourcesOutput schema from Amazon Proton API
layout: schema
name: ListServicePipelineProvisionedResourcesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: provisionedResources
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-service-pipeline-provisioned-resources-output-schema.json
slug: amazon-proton-list-service-pipeline-provisioned-resources-output
source_filename: amazon-proton-list-service-pipeline-provisioned-resources-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-pipeline-provisioned-resources-output-schema.json\",\n  \"title\": \"ListServicePipelineProvisionedResourcesOutput\",\n  \"description\": \"ListServicePipelineProvisionedResourcesOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyNextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next provisioned resource in the array of provisioned resources, after the current requested list of provisioned resources.\"\n        }\n      ]\n    },\n    \"provisionedResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedResourceList\"\n        },\n        {\n\
  \          \"description\": \"An array of provisioned resources for a service and pipeline.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"provisionedResources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-pipeline-provisioned-resources-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServicePipelineProvisionedResourcesOutput
---
