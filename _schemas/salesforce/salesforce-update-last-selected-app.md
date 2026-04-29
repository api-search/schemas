---
description: ''
layout: schema
name: UpdateLastSelectedApp
properties_list:
- description: ''
  name: appId
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: developerName
  type: string
- description: ''
  name: eTag
  type: string
- description: ''
  name: formFactors
  type: array
- description: ''
  name: headerColor
  type: string
- description: ''
  name: iconUrl
  type: string
- description: ''
  name: isNavAutoTempTabsDisabled
  type: boolean
- description: ''
  name: isNavPersonalizationDisabled
  type: boolean
- description: ''
  name: isNavTabPersistenceDisabled
  type: boolean
- description: ''
  name: label
  type: string
- description: ''
  name: logoUrl
  type: string
- description: ''
  name: mobileStartUrl
  type: '[''string'', ''null'']'
- description: ''
  name: navItems
  type: array
- description: ''
  name: selected
  type: boolean
- description: ''
  name: startUrl
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: userNavItems
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-update-last-selected-app-schema.json
slug: salesforce-update-last-selected-app
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"developerName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"formFactors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"headerColor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"isNavAutoTempTabsDisabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isNavPersonalizationDisabled\": {\n      \"type\": \"boolean\",\n   \
  \   \"example\": true\n    },\n    \"isNavTabPersistenceDisabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"logoUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"mobileStartUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"navItems\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"availableInClassic\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"availableInLightning\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"color\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n       \
  \   \"content\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"custom\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"iconUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"id\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"abc123\"\n          },\n          \"itemType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"objectApiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"objectLabel\": {\n   \
  \         \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"objectLabelPlural\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"pageReference\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"attributes\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"pageName\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"objectApiName\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"actionName\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                }\n              },\n              \"state\": {\n                \"type\"\
  : \"object\",\n                \"example\": \"example_value\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"attributes\",\n              \"state\",\n              \"type\"\n            ]\n          },\n          \"standardType\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"availableInClassic\",\n          \"availableInLightning\",\n          \"color\",\n          \"content\",\n          \"custom\",\n          \"developerName\",\n          \"iconUrl\",\n          \"id\",\n          \"itemType\",\n          \"label\",\n          \"objectApiName\",\n          \"objectLabel\",\n          \"objectLabelPlural\",\n          \"pageReference\",\n          \"standardType\"\n        ]\n      }\n    },\n    \"selected\": {\n\
  \      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"startUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"userNavItems\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"appId\",\n    \"description\",\n    \"developerName\",\n    \"eTag\",\n    \"formFactors\",\n    \"headerColor\",\n    \"iconUrl\",\n    \"isNavAutoTempTabsDisabled\",\n    \"isNavPersonalizationDisabled\",\n    \"isNavTabPersistenceDisabled\",\n    \"label\",\n    \"logoUrl\",\n    \"mobileStartUrl\",\n    \"navItems\",\n    \"selected\",\n    \"startUrl\",\n    \"type\",\n    \"userNavItems\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateLastSelectedApp\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-update-last-selected-app-schema.json
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
title: UpdateLastSelectedApp
---
