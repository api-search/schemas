---
description: Nielsen Naes Ii Nw
layout: schema
name: NielsenNaesIiNw
properties_list:
- description: ''
  name: CheckDigitString
  type: object
- description: ''
  name: Sid
  type: object
- description: ''
  name: Timezone
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-nielsen-naes-ii-nw-schema.json
slug: medialive-api-nielsen-naes-ii-nw
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-naes-ii-nw-schema.json\",\n  \"title\": \"NielsenNaesIiNw\",\n  \"description\": \"Nielsen Naes Ii Nw\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CheckDigitString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin2Max2\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"checkDigitString\"\n          },\n          \"description\": \"Enter the check digit string for the watermark\"\n        }\n      ]\n    },\n    \"Sid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin1Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sid\"\n          },\n          \"description\": \"Enter the Nielsen Source ID (SID) to include in the watermark\"\n      \
  \  }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenWatermarkTimezones\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timezone\"\n          },\n          \"description\": \"Choose the timezone for the time stamps in the watermark. If not provided,\\nthe timestamps will be in Coordinated Universal Time (UTC)\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CheckDigitString\",\n    \"Sid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-naes-ii-nw-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NielsenNaesIiNw
---
