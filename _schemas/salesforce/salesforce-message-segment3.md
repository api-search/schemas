---
description: ''
layout: schema
name: MessageSegment3
properties_list:
- description: ''
  name: text
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: altText
  type: '[''string'', ''null'']'
- description: ''
  name: htmlTag
  type: string
- description: ''
  name: markupType
  type: string
- description: ''
  name: url
  type: '[''string'', ''null'']'
- description: ''
  name: accessible
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: record
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-message-segment3-schema.json
slug: salesforce-message-segment3
source_filename: salesforce-message-segment3-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"altText\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"htmlTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"markupType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"accessible\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"record\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"additionalLabel\": {\n          \"type\": \"['string', 'null']\",\n          \"example\"\
  : \"example_value\"\n        },\n        \"communityNickname\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"companyName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"isActive\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isInThisCommunity\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"motif\": {\n          \"type\": \"object\",\n          \"properties\": {\n\
  \            \"color\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"largeIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"mediumIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"smallIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"svgIconUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            }\n          },\n          \"required\": [\n            \"color\",\n            \"largeIconUrl\",\n            \"mediumIconUrl\",\n            \"smallIconUrl\",\n            \"svgIconUrl\"\n          ]\n        },\n        \"mySubscription\": {\n          \"type\": \"['string', 'null']\",\n       \
  \   \"example\": \"example_value\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"outOfOffice\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"message\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"message\"\n          ]\n        },\n        \"photo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"fullEmailPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"user@example.com\"\n            },\n            \"largePhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"mediumPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"photoVersionId\"\
  : {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"smallPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"standardEmailPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"user@example.com\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            }\n          },\n          \"required\": [\n            \"fullEmailPhotoUrl\",\n            \"largePhotoUrl\",\n            \"mediumPhotoUrl\",\n            \"photoVersionId\",\n            \"smallPhotoUrl\",\n            \"standardEmailPhotoUrl\",\n            \"url\"\n          ]\n        },\n        \"reputation\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"title\": {\n          \"type\": \"['string', 'null']\"\
  ,\n          \"example\": \"Example Title\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"userType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"additionalLabel\",\n        \"communityNickname\",\n        \"companyName\",\n        \"displayName\",\n        \"firstName\",\n        \"id\",\n        \"isActive\",\n        \"isInThisCommunity\",\n        \"lastName\",\n        \"motif\",\n        \"mySubscription\",\n        \"name\",\n        \"outOfOffice\",\n        \"photo\",\n        \"reputation\",\n        \"title\",\n        \"type\",\n        \"url\",\n        \"userType\"\n      ]\n    }\n  },\n  \"required\": [\n    \"text\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"MessageSegment3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-message-segment3-schema.json
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
title: MessageSegment3
---
