---
description: ''
layout: schema
name: Compliance
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-compliance-schema.json
slug: zoominfo-compliance
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"result\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"input\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"companyname\": {\n                    \"type\": \"string\",\n                    \"example\": \"Acme Corporation\"\n                  },\n                  \"personfirstname\": {\n                    \"type\": \"string\",\n                    \"example\": \"Acme Corporation\"\n                  },\n                  \"personlastname\": {\n                    \"type\": \"string\",\n                    \"example\": \"Acme Corporation\"\n                \
  \  },\n                  \"personemailaddress\": {\n                    \"type\": \"string\",\n                    \"example\": \"jsmith@example.com\"\n                  }\n                }\n              },\n              \"data\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"object\"\n                    },\n                    \"firstName\": {\n                      \"type\": \"object\"\n                    },\n                    \"lastName\": {\n                      \"type\": \"object\"\n                    },\n                    \"title\": {\n                      \"type\": \"object\"\n                    },\n                    \"employmentHistory\": {\n                      \"type\": \"object\"\n                    },\n                \
  \    \"emailAddresses\": {\n                      \"type\": \"object\"\n                    },\n                    \"pastEmailAddresses\": {\n                      \"type\": \"object\"\n                    },\n                    \"withinEu\": {\n                      \"type\": \"object\"\n                    },\n                    \"hasCanadianEmail\": {\n                      \"type\": \"object\"\n                    },\n                    \"withinCalifornia\": {\n                      \"type\": \"object\"\n                    },\n                    \"withinCanada\": {\n                      \"type\": \"object\"\n                    },\n                    \"noticeProvidedDate\": {\n                      \"type\": \"object\"\n                    },\n                    \"hasMoved\": {\n                      \"type\": \"object\"\n                    },\n                    \"looksLikeEu\": {\n                      \"type\": \"object\"\n                    },\n                    \"\
  looksLikeCalifornia\": {\n                      \"type\": \"object\"\n                    },\n                    \"looksLikeCanada\": {\n                      \"type\": \"object\"\n                    },\n                    \"company\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"id\",\n                    \"firstName\",\n                    \"lastName\",\n                    \"title\",\n                    \"employmentHistory\",\n                    \"emailAddresses\",\n                    \"pastEmailAddresses\",\n                    \"withinEu\",\n                    \"hasCanadianEmail\",\n                    \"withinCalifornia\",\n                    \"withinCanada\",\n                    \"noticeProvidedDate\",\n                    \"hasMoved\",\n                    \"looksLikeEu\",\n                    \"looksLikeCalifornia\",\n                    \"looksLikeCanada\",\n     \
  \               \"company\"\n                  ]\n                }\n              }\n            },\n            \"required\": [\n              \"input\",\n              \"data\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"result\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Compliance\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-compliance-schema.json
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
title: Compliance
---
