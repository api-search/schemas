---
description: ''
layout: schema
name: SuccessfulFollowing-POST
properties_list:
- description: ''
  name: community
  type: '[''string'', ''null'']'
- description: ''
  name: id
  type: string
- description: ''
  name: subject
  type: object
- description: ''
  name: subscriber
  type: object
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-following-post-schema.json
slug: salesforce-successful-following-post
source_filename: salesforce-successful-following-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"community\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"subject\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"entityLabel\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"label\": {\n              \"type\": \"string\",\n              \"example\": \"Example Title\"\n            },\n            \"labelPlural\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"label\",\n            \"labelPlural\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"motif\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"color\": {\n\
  \              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"largeIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"mediumIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"smallIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"svgIconUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            }\n          },\n          \"required\": [\n            \"color\",\n            \"largeIconUrl\",\n            \"mediumIconUrl\",\n            \"smallIconUrl\",\n            \"svgIconUrl\"\n          ]\n        },\n        \"mySubscription\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\
  \n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"entityLabel\",\n        \"id\",\n        \"motif\",\n        \"mySubscription\",\n        \"name\",\n        \"type\",\n        \"url\"\n      ]\n    },\n    \"subscriber\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"additionalLabel\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"communityNickname\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"companyName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"displayName\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"isActive\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isInThisCommunity\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"motif\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"color\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"largeIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"mediumIconUrl\"\
  : {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"smallIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"svgIconUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            }\n          },\n          \"required\": [\n            \"color\",\n            \"largeIconUrl\",\n            \"mediumIconUrl\",\n            \"smallIconUrl\",\n            \"svgIconUrl\"\n          ]\n        },\n        \"mySubscription\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"outOfOffice\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"message\": {\n              \"type\": \"\
  string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"message\"\n          ]\n        },\n        \"photo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"fullEmailPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"user@example.com\"\n            },\n            \"largePhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"mediumPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"photoVersionId\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"500123\"\n            },\n            \"smallPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"standardEmailPhotoUrl\": {\n \
  \             \"type\": \"string\",\n              \"example\": \"user@example.com\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            }\n          },\n          \"required\": [\n            \"fullEmailPhotoUrl\",\n            \"largePhotoUrl\",\n            \"mediumPhotoUrl\",\n            \"photoVersionId\",\n            \"smallPhotoUrl\",\n            \"standardEmailPhotoUrl\",\n            \"url\"\n          ]\n        },\n        \"reputation\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"title\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"Example Title\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n\
  \        \"userType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"additionalLabel\",\n        \"communityNickname\",\n        \"companyName\",\n        \"displayName\",\n        \"firstName\",\n        \"id\",\n        \"isActive\",\n        \"isInThisCommunity\",\n        \"lastName\",\n        \"motif\",\n        \"mySubscription\",\n        \"name\",\n        \"outOfOffice\",\n        \"photo\",\n        \"reputation\",\n        \"title\",\n        \"type\",\n        \"url\",\n        \"userType\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"community\",\n    \"id\",\n    \"subject\",\n    \"subscriber\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulFollowing-POST\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-following-post-schema.json
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
title: SuccessfulFollowing-POST
---
