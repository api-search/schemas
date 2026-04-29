---
description: ListServiceTemplateVersionsOutput schema from Amazon Proton API
layout: schema
name: ListServiceTemplateVersionsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: templateVersions
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-service-template-versions-output-schema.json
slug: amazon-proton-list-service-template-versions-output
source_filename: amazon-proton-list-service-template-versions-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-template-versions-output-schema.json\",\n  \"title\": \"ListServiceTemplateVersionsOutput\",\n  \"description\": \"ListServiceTemplateVersionsOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next major or minor version in the array of major or minor versions of a service template, after the current requested list of service major or minor versions.\"\n        }\n      ]\n    },\n    \"templateVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplateVersionSummaryList\"\n        },\n        {\n\
  \          \"description\": \"An array of major or minor versions of a service template with detail data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"templateVersions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-template-versions-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServiceTemplateVersionsOutput
---
