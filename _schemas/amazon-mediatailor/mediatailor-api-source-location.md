---
description: A source location is a container for sources. For more information about source locations, see <a href="https://docs.aws.amazon.com/mediatailor/latest/ug/channel-assembly-source-locations.html">Working with source locations</a> in the <i>MediaTailor User Guide</i>.
layout: schema
name: SourceLocation
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
schema_file: json-schema/mediatailor-api-source-location-schema.json
slug: mediatailor-api-source-location
source_filename: mediatailor-api-source-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-source-location-schema.json\",\n  \"title\": \"SourceLocation\",\n  \"description\": \"A source location is a container for sources. For more information about source locations, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/channel-assembly-source-locations.html\\\">Working with source locations</a> in the <i>MediaTailor User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessConfiguration\"\n        },\n        {\n          \"description\": \"The access configuration for the source location.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n\
  \          \"description\": \"The ARN of the SourceLocation.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The timestamp that indicates when the source location was created.\"\n        }\n      ]\n    },\n    \"DefaultSegmentDeliveryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The default segment delivery configuration.\"\n        }\n      ]\n    },\n    \"HttpConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpConfiguration\"\n        },\n        {\n          \"description\": \"The HTTP configuration for the source location.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\
  \n        },\n        {\n          \"description\": \"The timestamp that indicates when the source location was last modified.\"\n        }\n      ]\n    },\n    \"SegmentDeliveryConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The segment delivery configurations for the source location.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the source location.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags assigned to the source location. Tags are key-value pairs that you can\
  \ associate with Amazon resources to help with organization, access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"HttpConfiguration\",\n    \"SourceLocationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-source-location-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: SourceLocation
---
