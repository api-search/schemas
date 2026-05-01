---
description: <p/>
layout: schema
name: DescribeComplianceByResourceResponse
properties_list:
- description: ''
  name: ComplianceByResources
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-compliance-by-resource-response-schema.json
slug: config-describe-compliance-by-resource-response
source_filename: config-describe-compliance-by-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-compliance-by-resource-response-schema.json\",\n  \"title\": \"DescribeComplianceByResourceResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceByResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceByResources\"\n        },\n        {\n          \"description\": \"Indicates whether the specified Amazon Web Services resource complies with all of the Config rules that evaluate it.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that you use in a subsequent request to get the next page of results in a paginated response.\"\n        }\n     \
  \ ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-compliance-by-resource-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeComplianceByResourceResponse
---
