---
description: VOD source configuration parameters.
layout: schema
name: VodSource
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
  name: SourceLocationName
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: VodSourceName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-vod-source-schema.json
slug: mediatailor-api-vod-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-vod-source-schema.json\",\n  \"title\": \"VodSource\",\n  \"description\": \"VOD source configuration parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The ARN for the VOD source.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The timestamp that indicates when the VOD source was created.\"\n        }\n      ]\n    },\n    \"HttpPackageConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPackageConfigurations\"\n        },\n\
  \        {\n          \"description\": \"The HTTP package configurations for the VOD source.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The timestamp that indicates when the VOD source was last modified.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the source location that the VOD source is associated with.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags assigned to the VOD source. Tags are key-value pairs that you can associate with Amazon resources\
  \ to help with organization, access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    },\n    \"VodSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the VOD source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"HttpPackageConfigurations\",\n    \"SourceLocationName\",\n    \"VodSourceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-vod-source-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VodSource
---
