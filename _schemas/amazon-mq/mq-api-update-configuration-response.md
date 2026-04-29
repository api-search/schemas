---
description: UpdateConfigurationResponse schema from Amazon MQ API
layout: schema
name: UpdateConfigurationResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: LatestRevision
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Warnings
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-update-configuration-response-schema.json
slug: mq-api-update-configuration-response
source_filename: mq-api-update-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-configuration-response-schema.json\",\n  \"title\": \"UpdateConfigurationResponse\",\n  \"description\": \"UpdateConfigurationResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"Required. The Amazon Resource Name (ARN) of the configuration.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"created\"\n          },\n          \"description\": \"Required. The date and time of the configuration.\"\
  \n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"Required. The unique ID that Amazon MQ generates for the configuration.\"\n        }\n      ]\n    },\n    \"LatestRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRevision\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"latestRevision\"\n          },\n          \"description\": \"The latest revision of the configuration.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Required. The name of the configuration. This value can contain only alphanumeric characters, dashes,\
  \ periods, underscores, and tildes (- . _ ~). This value must be 1-150 characters long.\"\n        }\n      ]\n    },\n    \"Warnings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSanitizationWarning\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"warnings\"\n          },\n          \"description\": \"The list of the first 20 warnings about the configuration XML elements or attributes that were sanitized.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-configuration-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateConfigurationResponse
---
