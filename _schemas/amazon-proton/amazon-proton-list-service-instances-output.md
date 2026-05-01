---
description: ListServiceInstancesOutput schema from Amazon Proton API
layout: schema
name: ListServiceInstancesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: serviceInstances
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-service-instances-output-schema.json
slug: amazon-proton-list-service-instances-output
source_filename: amazon-proton-list-service-instances-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instances-output-schema.json\",\n  \"title\": \"ListServiceInstancesOutput\",\n  \"description\": \"ListServiceInstancesOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next service instance in the array of service instances, after the current requested list of service instances.\"\n        }\n      ]\n    },\n    \"serviceInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceInstanceSummaryList\"\n        },\n        {\n          \"description\": \"An array of service instances with summary data.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceInstances\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instances-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServiceInstancesOutput
---
