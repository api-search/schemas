---
description: ListServiceTemplateVersionsInput schema from Amazon Proton API
layout: schema
name: ListServiceTemplateVersionsInput
properties_list:
- description: ''
  name: majorVersion
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-service-template-versions-input-schema.json
slug: amazon-proton-list-service-template-versions-input
source_filename: amazon-proton-list-service-template-versions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-template-versions-input-schema.json\",\n  \"title\": \"ListServiceTemplateVersionsInput\",\n  \"description\": \"ListServiceTemplateVersionsInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"majorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"<p>To view a list of minor of versions under a major version of a service template, include <code>major Version</code>.</p> <p>To view a list of major versions of a service template, <i>exclude</i> <code>major Version</code>.</p>\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPageResults\"\n        },\n\
  \        {\n          \"description\": \"The maximum number of major or minor versions of a service template to list.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next major or minor version in the array of major or minor versions of a service template, after the list of major or minor versions that was previously requested.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-template-versions-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServiceTemplateVersionsInput
---
