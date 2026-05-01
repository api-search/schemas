---
description: Filters the results based on account ID and region.
layout: schema
name: AggregateConformancePackComplianceSummaryFilters
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: AwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-conformance-pack-compliance-summary-filters-schema.json
slug: config-aggregate-conformance-pack-compliance-summary-filters
source_filename: config-aggregate-conformance-pack-compliance-summary-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-summary-filters-schema.json\",\n  \"title\": \"AggregateConformancePackComplianceSummaryFilters\",\n  \"description\": \"Filters the results based on account ID and region. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit Amazon Web Services account ID of the source account.\"\n        }\n      ]\n    },\n    \"AwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source Amazon Web Services Region from where the data is aggregated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-summary-filters-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateConformancePackComplianceSummaryFilters
---
