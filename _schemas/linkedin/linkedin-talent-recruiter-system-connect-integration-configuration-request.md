---
description: Request for syncing integration configurations
layout: schema
name: IntegrationConfigurationRequest
properties_list:
- description: ''
  name: entities
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-integration-configuration-request-schema.json
slug: linkedin-talent-recruiter-system-connect-integration-configuration-request
source_filename: linkedin-talent-recruiter-system-connect-integration-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-integration-configuration-request-schema.json\",\n  \"title\": \"IntegrationConfigurationRequest\",\n  \"description\": \"Request for syncing integration configurations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entities\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/ConfigurationValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-integration-configuration-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: IntegrationConfigurationRequest
---
