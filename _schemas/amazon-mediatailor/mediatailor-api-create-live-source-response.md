---
description: CreateLiveSourceResponse schema from Amazon MediaTailor API
layout: schema
name: CreateLiveSourceResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: HttpPackageConfigurations
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: LiveSourceName
  type: object
- description: ''
  name: SourceLocationName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-live-source-response-schema.json
slug: mediatailor-api-create-live-source-response
source_filename: mediatailor-api-create-live-source-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-live-source-response-schema.json\",\n  \"title\": \"CreateLiveSourceResponse\",\n  \"description\": \"CreateLiveSourceResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The ARN to assign to the live source.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time the live source was created.\"\n        }\n      ]\n    },\n    \"HttpPackageConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPackageConfigurations\"\
  \n        },\n        {\n          \"description\": \"A list of HTTP package configuration parameters for this live source.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time the live source was last modified.\"\n        }\n      ]\n    },\n    \"LiveSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name to assign to the live source.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name to assign to the source location of the live source.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags to assign to the live source. Tags are key-value pairs that you can associate with Amazon resources to help with organization, access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-live-source-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateLiveSourceResponse
---
