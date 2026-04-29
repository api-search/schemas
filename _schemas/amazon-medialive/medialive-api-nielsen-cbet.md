---
description: Nielsen CBET
layout: schema
name: NielsenCBET
properties_list:
- description: ''
  name: CbetCheckDigitString
  type: object
- description: ''
  name: CbetStepaside
  type: object
- description: ''
  name: Csid
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-nielsen-cbet-schema.json
slug: medialive-api-nielsen-cbet
source_filename: medialive-api-nielsen-cbet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-cbet-schema.json\",\n  \"title\": \"NielsenCBET\",\n  \"description\": \"Nielsen CBET\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CbetCheckDigitString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin2Max2\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cbetCheckDigitString\"\n          },\n          \"description\": \"Enter the CBET check digits to use in the watermark.\"\n        }\n      ]\n    },\n    \"CbetStepaside\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenWatermarksCbetStepaside\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cbetStepaside\"\n          },\n          \"description\": \"Determines the method of CBET insertion mode\
  \ when prior encoding is detected on the same layer.\"\n        }\n      ]\n    },\n    \"Csid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max7\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"csid\"\n          },\n          \"description\": \"Enter the CBET Source ID (CSID) to use in the watermark\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CbetCheckDigitString\",\n    \"CbetStepaside\",\n    \"Csid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-cbet-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NielsenCBET
---
