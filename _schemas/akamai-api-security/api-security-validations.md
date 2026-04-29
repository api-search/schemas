---
description: Contains warnings, errors, or notices determined by validating the match target.
layout: schema
name: validations
properties_list:
- description: The list of errors.
  name: errors
  type: array
- description: The list of notices.
  name: notices
  type: array
- description: The list of warnings.
  name: warnings
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-validations-schema.json
slug: api-security-validations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-validations-schema.json\",\n  \"title\": \"validations\",\n  \"description\": \"Contains warnings, errors, or notices determined by validating the match target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"description\": \"The list of errors.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains feedback on validation.\",\n        \"properties\": {\n          \"detail\": {\n            \"description\": \"The explanation of the error message.\",\n            \"type\": \"string\"\n          },\n          \"fieldName\": {\n            \"description\": \"The name of the field causing the validation problem.\",\n            \"type\": \"string\"\n          },\n          \"jsonReference\": {\n            \"description\"\
  : \"The JSON reference to the field in the resource.\",\n            \"type\": \"string\"\n          },\n          \"title\": {\n            \"description\": \"The title for the error.\",\n            \"example\": \"Not Found\",\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"description\": \"The URL for the error type.\",\n            \"example\": \"/appsec/problem-types/INCOMPATIBLE-FIELD\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"title\",\n          \"type\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/validation.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    },\n    \"notices\": {\n      \"description\": \"The list of notices.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains feedback on validation.\",\n        \"properties\": {\n          \"detail\": {\n           \
  \ \"description\": \"The explanation of the error message.\",\n            \"type\": \"string\"\n          },\n          \"fieldName\": {\n            \"description\": \"The name of the field causing the validation problem.\",\n            \"type\": \"string\"\n          },\n          \"jsonReference\": {\n            \"description\": \"The JSON reference to the field in the resource.\",\n            \"type\": \"string\"\n          },\n          \"title\": {\n            \"description\": \"The title for the error.\",\n            \"example\": \"Not Found\",\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"description\": \"The URL for the error type.\",\n            \"example\": \"/appsec/problem-types/INCOMPATIBLE-FIELD\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"title\",\n          \"type\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/validation.yaml\"\
  \n        }\n      },\n      \"type\": \"array\"\n    },\n    \"warnings\": {\n      \"description\": \"The list of warnings.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains feedback on validation.\",\n        \"properties\": {\n          \"detail\": {\n            \"description\": \"The explanation of the error message.\",\n            \"type\": \"string\"\n          },\n          \"fieldName\": {\n            \"description\": \"The name of the field causing the validation problem.\",\n            \"type\": \"string\"\n          },\n          \"jsonReference\": {\n            \"description\": \"The JSON reference to the field in the resource.\",\n            \"type\": \"string\"\n          },\n          \"title\": {\n            \"description\": \"The title for the error.\",\n            \"example\": \"Not Found\",\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"description\": \"The URL for the\
  \ error type.\",\n            \"example\": \"/appsec/problem-types/INCOMPATIBLE-FIELD\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"title\",\n          \"type\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/validation.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"notices\",\n    \"errors\",\n    \"warnings\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-validations-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: validations
---
