---
description: ConversionsByMemberCompanyResponse200 from LinkedIn API
layout: schema
name: ConversionsByMemberCompanyResponse200
properties_list:
- description: ''
  name: paging
  type: object
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-reporting-roi-conversions-by-member-company-response200-schema.json
slug: linkedin-marketing-reporting-roi-conversions-by-member-company-response200
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-reporting-roi-conversions-by-member-company-response200-schema.json\",\n  \"title\": \"ConversionsByMemberCompanyResponse200\",\n  \"description\": \"ConversionsByMemberCompanyResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"integer\"\n        },\n        \"count\": {\n          \"type\": \"integer\"\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"items\": {}\n        }\n      }\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"pivotValues\": {\n            \"type\": \"array\",\n            \"items\": {\n             \
  \ \"type\": \"string\"\n            }\n          },\n          \"externalWebsiteConversions\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-reporting-roi-conversions-by-member-company-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ConversionsByMemberCompanyResponse200
---
