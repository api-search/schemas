---
description: ''
layout: schema
name: Enrichcompaniesbyname
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-enrichcompaniesbyname-schema.json
slug: zoominfo-enrichcompaniesbyname
source_filename: zoominfo-enrichcompaniesbyname-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"outputFields\": {\n          \"type\": \"array\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"result\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"input\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"companyname\": {\n                    \"type\": \"string\",\n                    \"example\": \"Acme Corporation\"\n                  }\n                },\n                \"required\": [\n                \
  \  \"companyname\"\n                ]\n              },\n              \"data\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"object\"\n                    },\n                    \"ticker\": {\n                      \"type\": \"object\"\n                    },\n                    \"name\": {\n                      \"type\": \"object\"\n                    },\n                    \"website\": {\n                      \"type\": \"object\"\n                    },\n                    \"domainList\": {\n                      \"type\": \"object\"\n                    },\n                    \"logo\": {\n                      \"type\": \"object\"\n                    },\n                    \"socialMediaUrls\": {\n                      \"type\": \"object\"\
  \n                    },\n                    \"revenue\": {\n                      \"type\": \"object\"\n                    },\n                    \"employeeCount\": {\n                      \"type\": \"object\"\n                    },\n                    \"numberOfContactsInZoomInfo\": {\n                      \"type\": \"object\"\n                    },\n                    \"phone\": {\n                      \"type\": \"object\"\n                    },\n                    \"fax\": {\n                      \"type\": \"object\"\n                    },\n                    \"street\": {\n                      \"type\": \"object\"\n                    },\n                    \"city\": {\n                      \"type\": \"object\"\n                    },\n                    \"state\": {\n                      \"type\": \"object\"\n                    },\n                    \"zipCode\": {\n                      \"type\": \"object\"\n                    },\n                    \"country\"\
  : {\n                      \"type\": \"object\"\n                    },\n                    \"continent\": {\n                      \"type\": \"object\"\n                    },\n                    \"companyStatus\": {\n                      \"type\": \"object\"\n                    },\n                    \"companyStatusDate\": {\n                      \"type\": \"object\"\n                    },\n                    \"employeeGrowth\": {\n                      \"type\": \"object\"\n                    },\n                    \"type\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"id\",\n                    \"ticker\",\n                    \"name\",\n                    \"website\",\n                    \"domainList\",\n                    \"logo\",\n                    \"socialMediaUrls\",\n                    \"revenue\",\n                    \"employeeCount\",\n                 \
  \   \"numberOfContactsInZoomInfo\",\n                    \"phone\",\n                    \"fax\",\n                    \"street\",\n                    \"city\",\n                    \"state\",\n                    \"zipCode\",\n                    \"country\",\n                    \"continent\",\n                    \"companyStatus\",\n                    \"companyStatusDate\",\n                    \"employeeGrowth\",\n                    \"type\"\n                  ]\n                }\n              }\n            },\n            \"required\": [\n              \"input\",\n              \"data\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"outputFields\",\n        \"result\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enrichcompaniesbyname\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-enrichcompaniesbyname-schema.json
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
title: Enrichcompaniesbyname
---
