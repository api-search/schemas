---
description: ValidateTheUsersOrganizationResponse200 from LinkedIn API
layout: schema
name: ValidateTheUsersOrganizationResponse200
properties_list:
- description: ''
  name: paging
  type: object
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-leads-validate-the-users-organization-response200-schema.json
slug: linkedin-marketing-leads-validate-the-users-organization-response200
source_filename: linkedin-marketing-leads-validate-the-users-organization-response200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-leads-validate-the-users-organization-response200-schema.json\",\n  \"title\": \"ValidateTheUsersOrganizationResponse200\",\n  \"description\": \"ValidateTheUsersOrganizationResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"integer\"\n        },\n        \"count\": {\n          \"type\": \"integer\"\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"items\": {}\n        }\n      }\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"roleAssignee\": {\n            \"type\": \"string\"\n          },\n          \"state\": {\n  \
  \          \"type\": \"string\"\n          },\n          \"lastModified\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"actor\": {\n                \"type\": \"string\"\n              },\n              \"impersonator\": {\n                \"type\": \"string\"\n              },\n              \"time\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"role\": {\n            \"type\": \"string\"\n          },\n          \"created\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"actor\": {\n                \"type\": \"string\"\n              },\n              \"impersonator\": {\n                \"type\": \"string\"\n              },\n              \"time\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"organization\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-leads-validate-the-users-organization-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ValidateTheUsersOrganizationResponse200
---
