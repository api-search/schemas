---
description: ''
layout: schema
name: GetActiveTheme
properties_list:
- description: ''
  name: brandColor
  type: string
- description: ''
  name: brandImage
  type: object
- description: ''
  name: defaultGroupBanner
  type: object
- description: ''
  name: defaultGroupImage
  type: object
- description: ''
  name: defaultPageBanner
  type: object
- description: ''
  name: defaultUserBanner
  type: object
- description: ''
  name: defaultUserImage
  type: object
- description: ''
  name: density
  type: string
- description: ''
  name: headerColor
  type: string
- description: ''
  name: linkColor
  type: string
- description: ''
  name: pageColor
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-active-theme-schema.json
slug: salesforce-get-active-theme
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"brandColor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"brandImage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"largeUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"mediumUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"smallUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"largeUrl\",\n        \"mediumUrl\",\n        \"smallUrl\"\n      ]\n    },\n    \"defaultGroupBanner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fullSizeUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"fullSizeUrl\"\n      ]\n  \
  \  },\n    \"defaultGroupImage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"largeUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"mediumUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"smallUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"largeUrl\",\n        \"mediumUrl\",\n        \"smallUrl\"\n      ]\n    },\n    \"defaultPageBanner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fullSizeUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"fullSizeUrl\"\n      ]\n    },\n    \"defaultUserBanner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fullSizeUrl\": {\n          \"type\": \"string\"\
  ,\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"fullSizeUrl\"\n      ]\n    },\n    \"defaultUserImage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"largeUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"mediumUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"smallUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"largeUrl\",\n        \"mediumUrl\",\n        \"smallUrl\"\n      ]\n    },\n    \"density\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"headerColor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"linkColor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n\
  \    \"pageColor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"brandColor\",\n    \"brandImage\",\n    \"defaultGroupBanner\",\n    \"defaultGroupImage\",\n    \"defaultPageBanner\",\n    \"defaultUserBanner\",\n    \"defaultUserImage\",\n    \"density\",\n    \"headerColor\",\n    \"linkColor\",\n    \"pageColor\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetActiveTheme\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-active-theme-schema.json
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
title: GetActiveTheme
---
