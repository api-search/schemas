---
description: PutOrganizationConformancePackResponse schema
layout: schema
name: PutOrganizationConformancePackResponse
properties_list:
- description: ''
  name: OrganizationConformancePackArn
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-organization-conformance-pack-response-schema.json
slug: config-put-organization-conformance-pack-response
source_filename: config-put-organization-conformance-pack-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-conformance-pack-response-schema.json\",\n  \"title\": \"PutOrganizationConformancePackResponse\",\n  \"description\": \"PutOrganizationConformancePackResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"ARN of the organization conformance pack.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-conformance-pack-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutOrganizationConformancePackResponse
---
