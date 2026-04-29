---
description: Request for updating ATS integrations
layout: schema
name: AtsIntegrationUpdateRequest
properties_list:
- description: ''
  name: entities
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-ats-integration-update-request-schema.json
slug: linkedin-talent-recruiter-system-connect-ats-integration-update-request
source_filename: linkedin-talent-recruiter-system-connect-ats-integration-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-ats-integration-update-request-schema.json\",\n  \"title\": \"AtsIntegrationUpdateRequest\",\n  \"description\": \"Request for updating ATS integrations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entities\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/IntegrationPatch\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-ats-integration-update-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AtsIntegrationUpdateRequest
---
