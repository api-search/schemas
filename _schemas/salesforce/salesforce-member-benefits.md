---
description: ''
layout: schema
name: MemberBenefits
properties_list:
- description: ''
  name: memberBenefits
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-member-benefits-schema.json
slug: salesforce-member-benefits
source_filename: salesforce-member-benefits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"memberBenefits\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"benefitId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"benefitName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"benefitTypeId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"benefitTypeName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"createdRecordId\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"500123\"\n          },\n          \"createdRecordName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n\
  \          \"description\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"A sample description.\"\n          },\n          \"endDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"isActive\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"memberBenefitStatus\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"startDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"benefitId\",\n          \"benefitName\",\n          \"benefitTypeId\",\n          \"benefitTypeName\",\n          \"createdRecordId\",\n          \"createdRecordName\",\n          \"description\",\n          \"endDate\",\n          \"isActive\",\n          \"memberBenefitStatus\",\n         \
  \ \"startDate\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"memberBenefits\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemberBenefits\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-member-benefits-schema.json
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
title: MemberBenefits
---
