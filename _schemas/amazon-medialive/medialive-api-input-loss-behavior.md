---
description: Input Loss Behavior
layout: schema
name: InputLossBehavior
properties_list:
- description: ''
  name: BlackFrameMsec
  type: object
- description: ''
  name: InputLossImageColor
  type: object
- description: ''
  name: InputLossImageSlate
  type: object
- description: ''
  name: InputLossImageType
  type: object
- description: ''
  name: RepeatFrameMsec
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-loss-behavior-schema.json
slug: medialive-api-input-loss-behavior
source_filename: medialive-api-input-loss-behavior-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-loss-behavior-schema.json\",\n  \"title\": \"InputLossBehavior\",\n  \"description\": \"Input Loss Behavior\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlackFrameMsec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blackFrameMsec\"\n          },\n          \"description\": \"Documentation update needed\"\n        }\n      ]\n    },\n    \"InputLossImageColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin6Max6\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossImageColor\"\n          },\n          \"description\": \"When input loss image type is \\\"color\\\" this field specifies\
  \ the color to use. Value: 6 hex characters representing the values of RGB.\"\n        }\n      ]\n    },\n    \"InputLossImageSlate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossImageSlate\"\n          },\n          \"description\": \"When input loss image type is \\\"slate\\\" these fields specify the parameters for accessing the slate.\"\n        }\n      ]\n    },\n    \"InputLossImageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLossImageType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossImageType\"\n          },\n          \"description\": \"Indicates whether to substitute a solid color or a slate into the output after input loss exceeds blackFrameMsec.\"\n        }\n      ]\n    },\n    \"RepeatFrameMsec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000000\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"repeatFrameMsec\"\n          },\n          \"description\": \"Documentation update needed\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-loss-behavior-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputLossBehavior
---
