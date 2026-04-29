---
description: <p/>
layout: schema
name: GetComplianceDetailsByResourceRequest
properties_list:
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ComplianceTypes
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ResourceEvaluationId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-compliance-details-by-resource-request-schema.json
slug: config-get-compliance-details-by-resource-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-details-by-resource-request-schema.json\",\n  \"title\": \"GetComplianceDetailsByResourceRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The type of the Amazon Web Services resource for which you want compliance information.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services resource for which you want compliance information.\"\n        }\n      ]\n    },\n    \"ComplianceTypes\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceTypes\"\n        },\n        {\n          \"description\": \"<p>Filters the results by compliance.</p> <p> <code>INSUFFICIENT_DATA</code> is a valid <code>ComplianceType</code> that is returned when an Config rule cannot be evaluated. However, <code>INSUFFICIENT_DATA</code> cannot be used as a <code>ComplianceType</code> for filtering results.</p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    },\n    \"ResourceEvaluationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationId\"\n        },\n        {\n          \"description\": \"<p>The unique ID of Amazon Web Services\
  \ resource execution for which you want to retrieve evaluation results. </p> <note> <p>You need to only provide either a <code>ResourceEvaluationID</code> or a <code>ResourceID </code>and <code>ResourceType</code>.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-details-by-resource-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetComplianceDetailsByResourceRequest
---
