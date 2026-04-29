---
description: Alert configuration parameters.
layout: schema
name: Alert
properties_list:
- description: ''
  name: AlertCode
  type: object
- description: ''
  name: AlertMessage
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: RelatedResourceArns
  type: object
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-alert-schema.json
slug: mediatailor-api-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-alert-schema.json\",\n  \"title\": \"Alert\",\n  \"description\": \"Alert configuration parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlertCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The code for the alert. For example, <code>NOT_PROCESSED</code>.\"\n        }\n      ]\n    },\n    \"AlertMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"If an alert is generated for a resource, an explanation of the reason for the alert.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\
  \n        },\n        {\n          \"description\": \"The timestamp when the alert was last modified.\"\n        }\n      ]\n    },\n    \"RelatedResourceArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Names (ARNs) related to this alert.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AlertCode\",\n    \"AlertMessage\",\n    \"LastModifiedTime\",\n    \"RelatedResourceArns\",\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-alert-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Alert
---
