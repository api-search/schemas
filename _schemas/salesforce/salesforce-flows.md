---
description: ''
layout: schema
name: Flows
properties_list:
- description: ''
  name: implicit
  type: object
- description: ''
  name: password
  type: object
- description: ''
  name: authorizationCode
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-flows-schema.json
slug: salesforce-flows
source_filename: salesforce-flows-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"implicit\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"authorizationUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"scopes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"visualforce\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"address\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"custom_permissions\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"openid\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"profile\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n      \
  \      \"refresh_token\": {\n              \"type\": \"string\",\n              \"example\": \"CAUQAA\"\n            },\n            \"wave_api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"web\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"phone\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"offline_access\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"chatter_api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n\
  \            \"eclair_api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"example\": \"user@example.com\"\n            },\n            \"pardot_api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"full\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"visualforce\",\n            \"address\",\n            \"custom_permissions\",\n            \"openid\",\n            \"profile\",\n            \"refresh_token\",\n            \"wave_api\",\n            \"web\",\n            \"phone\",\n            \"offline_access\",\n            \"chatter_api\",\n            \"id\",\n            \"api\",\n            \"eclair_api\",\n            \"email\",\n            \"pardot_api\",\n         \
  \   \"full\"\n          ]\n        }\n      },\n      \"required\": [\n        \"authorizationUrl\",\n        \"scopes\"\n      ]\n    },\n    \"password\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tokenUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"scopes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"api\"\n          ]\n        }\n      },\n      \"required\": [\n        \"tokenUrl\",\n        \"scopes\"\n      ]\n    },\n    \"authorizationCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"authorizationUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"tokenUrl\": {\n          \"type\": \"string\",\n     \
  \     \"example\": \"https://www.example.com\"\n        },\n        \"scopes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"visualforce\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"address\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"custom_permissions\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"openid\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"profile\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"refresh_token\": {\n              \"type\": \"string\",\n              \"example\": \"CAUQAA\"\n            },\n            \"wave_api\": {\n              \"type\": \"string\",\n              \"example\"\
  : \"example_value\"\n            },\n            \"web\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"phone\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"offline_access\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"chatter_api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"eclair_api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"example\"\
  : \"user@example.com\"\n            },\n            \"pardot_api\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"full\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"visualforce\",\n            \"address\",\n            \"custom_permissions\",\n            \"openid\",\n            \"profile\",\n            \"refresh_token\",\n            \"wave_api\",\n            \"web\",\n            \"phone\",\n            \"offline_access\",\n            \"chatter_api\",\n            \"id\",\n            \"api\",\n            \"eclair_api\",\n            \"email\",\n            \"pardot_api\",\n            \"full\"\n          ]\n        }\n      },\n      \"required\": [\n        \"authorizationUrl\",\n        \"tokenUrl\",\n        \"scopes\"\n      ]\n    }\n  },\n  \"required\": [\n    \"implicit\",\n    \"password\"\
  ,\n    \"authorizationCode\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Flows\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-flows-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Flows
---
