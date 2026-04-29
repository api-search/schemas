---
description: CreateVodSourceRequest schema from Amazon MediaTailor API
layout: schema
name: CreateVodSourceRequest
properties_list:
- description: ''
  name: HttpPackageConfigurations
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-vod-source-request-schema.json
slug: mediatailor-api-create-vod-source-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-vod-source-request-schema.json\",\n  \"title\": \"CreateVodSourceRequest\",\n  \"description\": \"CreateVodSourceRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpPackageConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPackageConfigurations\"\n        },\n        {\n          \"description\": \"A list of HTTP package configuration parameters for this VOD source.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags to assign to the VOD source. Tags are key-value pairs\
  \ that you can associate with Amazon resources to help with organization, access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HttpPackageConfigurations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-vod-source-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateVodSourceRequest
---
