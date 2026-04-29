---
description: IntegrationPatch from LinkedIn API
layout: schema
name: IntegrationPatch
properties_list:
- description: ''
  name: patch
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-integration-patch-schema.json
slug: linkedin-talent-recruiter-system-connect-integration-patch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-integration-patch-schema.json\",\n  \"title\": \"IntegrationPatch\",\n  \"description\": \"IntegrationPatch from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"patch\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"$set\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"integrationName\": {\n              \"type\": \"string\",\n              \"example\": \"Customer Name LinkedIn Recruiter CSA_API Integration\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-integration-patch-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: IntegrationPatch
---
