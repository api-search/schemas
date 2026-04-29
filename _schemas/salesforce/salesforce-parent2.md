---
description: ''
layout: schema
name: Parent2
properties_list:
- description: ''
  name: entityLabel
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: motif
  type: object
- description: ''
  name: mySubscription
  type: '[''string'', ''null'']'
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: additionalLabel
  type: '[''string'', ''null'']'
- description: ''
  name: communityNickname
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: isActive
  type: boolean
- description: ''
  name: isInThisCommunity
  type: boolean
- description: ''
  name: lastName
  type: string
- description: ''
  name: outOfOffice
  type: object
- description: ''
  name: photo
  type: object
- description: ''
  name: reputation
  type: '[''string'', ''null'']'
- description: ''
  name: title
  type: '[''string'', ''null'']'
- description: ''
  name: userType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-parent2-schema.json
slug: salesforce-parent2
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityLabel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"labelPlural\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"label\",\n        \"labelPlural\"\n      ]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"motif\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"color\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"largeIconUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"mediumIconUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"smallIconUrl\":\
  \ {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"svgIconUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"color\",\n        \"largeIconUrl\",\n        \"mediumIconUrl\",\n        \"smallIconUrl\",\n        \"svgIconUrl\"\n      ]\n    },\n    \"mySubscription\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"additionalLabel\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"communityNickname\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isInThisCommunity\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"outOfOffice\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"message\"\n      ]\n    },\n    \"photo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fullEmailPhotoUrl\": {\n          \"type\": \"string\",\n    \
  \      \"example\": \"user@example.com\"\n        },\n        \"largePhotoUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"mediumPhotoUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"photoVersionId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"smallPhotoUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"standardEmailPhotoUrl\": {\n          \"type\": \"string\",\n          \"example\": \"user@example.com\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"fullEmailPhotoUrl\",\n        \"largePhotoUrl\",\n        \"mediumPhotoUrl\",\n        \"photoVersionId\",\n        \"smallPhotoUrl\",\n        \"standardEmailPhotoUrl\"\
  ,\n        \"url\"\n      ]\n    },\n    \"reputation\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"title\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"Example Title\"\n    },\n    \"userType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"motif\",\n    \"mySubscription\",\n    \"name\",\n    \"type\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parent2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-parent2-schema.json
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
title: Parent2
---
