---
description: UpdateSourceLocationRequest schema from Amazon MediaTailor API
layout: schema
name: UpdateSourceLocationRequest
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
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-update-source-location-request-schema.json
slug: mediatailor-api-update-source-location-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-source-location-request-schema.json\",\n  \"title\": \"UpdateSourceLocationRequest\",\n  \"description\": \"UpdateSourceLocationRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessConfiguration\"\n        },\n        {\n          \"description\": \"Access configuration parameters. Configures the type of authentication used to access content from your source location.\"\n        }\n      ]\n    },\n    \"DefaultSegmentDeliveryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The optional configuration\
  \ for the host server that serves segments.\"\n        }\n      ]\n    },\n    \"HttpConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpConfiguration\"\n        },\n        {\n          \"description\": \"The HTTP configuration for the source location.\"\n        }\n      ]\n    },\n    \"SegmentDeliveryConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSegmentDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"A list of the segment delivery configurations associated with this resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HttpConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-source-location-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateSourceLocationRequest
---
