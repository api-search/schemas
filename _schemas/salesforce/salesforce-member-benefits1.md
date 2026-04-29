---
description: ''
layout: schema
name: MemberBenefits1
properties_list:
- description: ''
  name: benefitId
  type: string
- description: ''
  name: benefitName
  type: string
- description: ''
  name: benefitTypeId
  type: string
- description: ''
  name: benefitTypeName
  type: string
- description: ''
  name: createdRecordId
  type: '[''string'', ''null'']'
- description: ''
  name: createdRecordName
  type: '[''string'', ''null'']'
- description: ''
  name: description
  type: '[''string'', ''null'']'
- description: ''
  name: endDate
  type: '[''string'', ''null'']'
- description: ''
  name: isActive
  type: boolean
- description: ''
  name: memberBenefitStatus
  type: '[''string'', ''null'']'
- description: ''
  name: startDate
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-member-benefits1-schema.json
slug: salesforce-member-benefits1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"benefitId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"benefitName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"benefitTypeId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"benefitTypeName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"createdRecordId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"createdRecordName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"A sample description.\"\n    },\n    \"endDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"memberBenefitStatus\"\
  : {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"startDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"benefitId\",\n    \"benefitName\",\n    \"benefitTypeId\",\n    \"benefitTypeName\",\n    \"createdRecordId\",\n    \"createdRecordName\",\n    \"description\",\n    \"endDate\",\n    \"isActive\",\n    \"memberBenefitStatus\",\n    \"startDate\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemberBenefits1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-member-benefits1-schema.json
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
title: MemberBenefits1
---
