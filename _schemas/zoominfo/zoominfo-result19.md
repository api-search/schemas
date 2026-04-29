---
description: ''
layout: schema
name: Result19
properties_list:
- description: ''
  name: input
  type: object
- description: ''
  name: data
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-result19-schema.json
slug: zoominfo-result19
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"companyname\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"personfirstname\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"personlastname\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"personemailaddress\": {\n          \"type\": \"string\",\n          \"example\": \"jsmith@example.com\"\n        }\n      }\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"firstName\": {\n            \"type\": \"string\",\n            \"example\"\
  : \"Acme Corporation\"\n          },\n          \"lastName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"example\": \"Vice President of Sales\"\n          },\n          \"employmentHistory\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"companyName\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"title\": {\n                  \"type\": \"string\",\n                  \"example\": \"Vice President of Sales\"\n                }\n              },\n              \"required\": [\n                \"companyName\",\n                \"title\"\n              ]\n            }\n          },\n          \"emailAddresses\"\
  : {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": \"user@example.com\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"pastEmailAddresses\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": \"user@example.com\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"withinEu\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"hasCanadianEmail\": {\n            \"type\": \"string\",\n            \"example\": \"jsmith@example.com\"\n          },\n          \"withinCalifornia\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"withinCanada\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"noticeProvidedDate\": {\n            \"type\": \"string\",\n\
  \            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"hasMoved\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"looksLikeEu\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"looksLikeCalifornia\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"looksLikeCanada\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"company\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"firstName\",\n          \"lastName\",\n  \
  \        \"title\",\n          \"employmentHistory\",\n          \"emailAddresses\",\n          \"pastEmailAddresses\",\n          \"withinEu\",\n          \"hasCanadianEmail\",\n          \"withinCalifornia\",\n          \"withinCanada\",\n          \"noticeProvidedDate\",\n          \"hasMoved\",\n          \"looksLikeEu\",\n          \"looksLikeCalifornia\",\n          \"looksLikeCanada\",\n          \"company\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"input\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Result19\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-result19-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: Result19
---
