---
description: ListServicesOutput schema from Amazon Proton API
layout: schema
name: ListServicesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: services
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-services-output-schema.json
slug: amazon-proton-list-services-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-services-output-schema.json\",\n  \"title\": \"ListServicesOutput\",\n  \"description\": \"ListServicesOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next service in the array of services, after the current requested list of services.\"\n        }\n      ]\n    },\n    \"services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceSummaryList\"\n        },\n        {\n          \"description\": \"An array of services with summaries of detail data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"services\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-services-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServicesOutput
---
