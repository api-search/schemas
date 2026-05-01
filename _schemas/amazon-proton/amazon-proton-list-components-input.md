---
description: ListComponentsInput schema from Amazon Proton API
layout: schema
name: ListComponentsInput
properties_list:
- description: ''
  name: environmentName
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-components-input-schema.json
slug: amazon-proton-list-components-input
source_filename: amazon-proton-list-components-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-components-input-schema.json\",\n  \"title\": \"ListComponentsInput\",\n  \"description\": \"ListComponentsInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of an environment for result list filtering. Proton returns components associated with the environment or attached to service instances running in it.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPageResults\"\n        },\n        {\n          \"description\": \"The maximum number of components to list.\"\n        }\n      ]\n    },\n \
  \   \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next component in the array of components, after the list of components that was previously requested.\"\n        }\n      ]\n    },\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of a service instance for result list filtering. Proton returns the component attached to the service instance, if any.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of a service for result list filtering. Proton returns components attached to service instances of the service.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-components-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListComponentsInput
---
