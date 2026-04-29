---
description: GetOrganizationConformancePackDetailedStatusRequest schema
layout: schema
name: GetOrganizationConformancePackDetailedStatusRequest
properties_list:
- description: ''
  name: OrganizationConformancePackName
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-organization-conformance-pack-detailed-status-request-schema.json
slug: config-get-organization-conformance-pack-detailed-status-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-conformance-pack-detailed-status-request-schema.json\",\n  \"title\": \"GetOrganizationConformancePackDetailedStatusRequest\",\n  \"description\": \"GetOrganizationConformancePackDetailedStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePackName\"\n        },\n        {\n          \"description\": \"The name of organization conformance pack for which you want status details for member accounts.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationResourceDetailedStatusFilters\"\n        },\n        {\n          \"description\": \"An <code>OrganizationResourceDetailedStatusFilters</code>\
  \ object.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CosmosPageLimit\"\n        },\n        {\n          \"description\": \"The maximum number of <code>OrganizationConformancePackDetailedStatuses</code> returned on each page. If you do not specify a number, Config uses the default. The default is 100. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The nextToken string returned on a previous page that you use to get the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConformancePackName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-conformance-pack-detailed-status-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetOrganizationConformancePackDetailedStatusRequest
---
