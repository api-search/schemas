---
description: CreateSourceLocationRequest schema from Amazon MediaTailor API
layout: schema
name: CreateSourceLocationRequest
properties_list:
- description: ''
  name: AccessConfiguration
  type: object
- description: ''
  name: DefaultSegmentDeliveryConfiguration
  type: object
- description: ''
  name: HttpConfiguration
  type: object
- description: ''
  name: SegmentDeliveryConfigurations
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-source-location-request-schema.json
slug: mediatailor-api-create-source-location-request
source_filename: mediatailor-api-create-source-location-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-source-location-request-schema.json\",\n  \"title\": \"CreateSourceLocationRequest\",\n  \"description\": \"CreateSourceLocationRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessConfiguration\"\n        },\n        {\n          \"description\": \"Access configuration parameters. Configures the type of authentication used to access content from your source location.\"\n        }\n      ]\n    },\n    \"DefaultSegmentDeliveryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The optional configuration\
  \ for the server that serves segments.\"\n        }\n      ]\n    },\n    \"HttpConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpConfiguration\"\n        },\n        {\n          \"description\": \"The source's HTTP package configurations.\"\n        }\n      ]\n    },\n    \"SegmentDeliveryConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"A list of the segment delivery configurations associated with this resource.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags to assign to the source location. Tags are key-value pairs that you can associate with Amazon resources to help with organization,\
  \ access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HttpConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-source-location-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateSourceLocationRequest
---
