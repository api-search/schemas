---
description: SearchVulnerabilitiesResponse schema
layout: schema
name: SearchVulnerabilitiesResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: vulnerabilities
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-search-vulnerabilities-response-schema.json
slug: inspector-search-vulnerabilities-response
source_filename: inspector-search-vulnerabilities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-search-vulnerabilities-response-schema.json\",\n  \"title\": \"SearchVulnerabilitiesResponse\",\n  \"description\": \"SearchVulnerabilitiesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination parameter to be used on the next list operation to retrieve more items.\"\n        }\n      ]\n    },\n    \"vulnerabilities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vulnerabilities\"\n        },\n        {\n          \"description\": \"Details about the listed vulnerability.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vulnerabilities\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-search-vulnerabilities-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: SearchVulnerabilitiesResponse
---
