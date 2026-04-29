---
description: DescribeOrganizationConformancePacksResponse schema
layout: schema
name: DescribeOrganizationConformancePacksResponse
properties_list:
- description: ''
  name: OrganizationConformancePacks
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-organization-conformance-packs-response-schema.json
slug: config-describe-organization-conformance-packs-response
source_filename: config-describe-organization-conformance-packs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-conformance-packs-response-schema.json\",\n  \"title\": \"DescribeOrganizationConformancePacksResponse\",\n  \"description\": \"DescribeOrganizationConformancePacksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePacks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePacks\"\n        },\n        {\n          \"description\": \"Returns a list of OrganizationConformancePacks objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The nextToken string returned on a previous page that you use to get the next page of results in a paginated response.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-conformance-packs-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeOrganizationConformancePacksResponse
---
