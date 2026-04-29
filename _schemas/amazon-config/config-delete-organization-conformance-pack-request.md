---
description: DeleteOrganizationConformancePackRequest schema
layout: schema
name: DeleteOrganizationConformancePackRequest
properties_list:
- description: ''
  name: OrganizationConformancePackName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-organization-conformance-pack-request-schema.json
slug: config-delete-organization-conformance-pack-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-organization-conformance-pack-request-schema.json\",\n  \"title\": \"DeleteOrganizationConformancePackRequest\",\n  \"description\": \"DeleteOrganizationConformancePackRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePackName\"\n        },\n        {\n          \"description\": \"The name of organization conformance pack that you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConformancePackName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-organization-conformance-pack-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteOrganizationConformancePackRequest
---
