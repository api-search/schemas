---
description: GetOrganizationConformancePackDetailedStatusResponse schema
layout: schema
name: GetOrganizationConformancePackDetailedStatusResponse
properties_list:
- description: ''
  name: OrganizationConformancePackDetailedStatuses
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-organization-conformance-pack-detailed-status-response-schema.json
slug: config-get-organization-conformance-pack-detailed-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-conformance-pack-detailed-status-response-schema.json\",\n  \"title\": \"GetOrganizationConformancePackDetailedStatusResponse\",\n  \"description\": \"GetOrganizationConformancePackDetailedStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackDetailedStatuses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePackDetailedStatuses\"\n        },\n        {\n          \"description\": \"A list of <code>OrganizationConformancePackDetailedStatus</code> objects. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The nextToken string returned on a previous\
  \ page that you use to get the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-conformance-pack-detailed-status-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetOrganizationConformancePackDetailedStatusResponse
---
