---
description: DescribeOrganizationConformancePackStatusesResponse schema
layout: schema
name: DescribeOrganizationConformancePackStatusesResponse
properties_list:
- description: ''
  name: OrganizationConformancePackStatuses
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-organization-conformance-pack-statuses-response-schema.json
slug: config-describe-organization-conformance-pack-statuses-response
source_filename: config-describe-organization-conformance-pack-statuses-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-conformance-pack-statuses-response-schema.json\",\n  \"title\": \"DescribeOrganizationConformancePackStatusesResponse\",\n  \"description\": \"DescribeOrganizationConformancePackStatusesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackStatuses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePackStatuses\"\n        },\n        {\n          \"description\": \"A list of <code>OrganizationConformancePackStatus</code> objects. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The nextToken string returned on a previous page that you use to\
  \ get the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-conformance-pack-statuses-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeOrganizationConformancePackStatusesResponse
---
