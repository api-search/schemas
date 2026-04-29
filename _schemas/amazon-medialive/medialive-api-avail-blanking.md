---
description: Avail Blanking
layout: schema
name: AvailBlanking
properties_list:
- description: ''
  name: AvailBlankingImage
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-avail-blanking-schema.json
slug: medialive-api-avail-blanking
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-avail-blanking-schema.json\",\n  \"title\": \"AvailBlanking\",\n  \"description\": \"Avail Blanking\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailBlankingImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availBlankingImage\"\n          },\n          \"description\": \"Blanking image to be used. Leave empty for solid black. Only bmp and png images are supported.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailBlankingState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"When set to enabled, causes video,\
  \ audio and captions to be blanked when insertion metadata is added.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-avail-blanking-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvailBlanking
---
