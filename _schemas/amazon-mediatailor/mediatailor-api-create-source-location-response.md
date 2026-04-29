---
description: CreateSourceLocationResponse schema from Amazon MediaTailor API
layout: schema
name: CreateSourceLocationResponse
properties_list:
- description: ''
  name: AccessConfiguration
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: DefaultSegmentDeliveryConfiguration
  type: object
- description: ''
  name: HttpConfiguration
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: SegmentDeliveryConfigurations
  type: object
- description: ''
  name: SourceLocationName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-source-location-response-schema.json
slug: mediatailor-api-create-source-location-response
source_filename: mediatailor-api-create-source-location-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-source-location-response-schema.json\",\n  \"title\": \"CreateSourceLocationResponse\",\n  \"description\": \"CreateSourceLocationResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessConfiguration\"\n        },\n        {\n          \"description\": \"Access configuration parameters. Configures the type of authentication used to access content from your source location.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The ARN to assign to the source location.\"\n        }\n      ]\n    },\n  \
  \  \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time the source location was created.\"\n        }\n      ]\n    },\n    \"DefaultSegmentDeliveryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The optional configuration for the server that serves segments.\"\n        }\n      ]\n    },\n    \"HttpConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpConfiguration\"\n        },\n        {\n          \"description\": \"The source's HTTP package configurations.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time the source location\
  \ was last modified.\"\n        }\n      ]\n    },\n    \"SegmentDeliveryConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The segment delivery configurations for the source location. For information about MediaTailor configurations, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/configurations.html\\\">Working with configurations in AWS Elemental MediaTailor</a>.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name to assign to the source location.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n \
  \         \"description\": \"The tags to assign to the source location. Tags are key-value pairs that you can associate with Amazon resources to help with organization, access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-source-location-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateSourceLocationResponse
---
