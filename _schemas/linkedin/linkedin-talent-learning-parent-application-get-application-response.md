---
description: Response containing application credentials and details
layout: schema
name: GetApplicationResponse
properties_list:
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-learning-parent-application-get-application-response-schema.json
slug: linkedin-talent-learning-parent-application-get-application-response
source_filename: linkedin-talent-learning-parent-application-get-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-get-application-response-schema.json\",\n  \"title\": \"GetApplicationResponse\",\n  \"description\": \"Response containing application credentials and details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApplicationCredentials\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-get-application-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: GetApplicationResponse
---
