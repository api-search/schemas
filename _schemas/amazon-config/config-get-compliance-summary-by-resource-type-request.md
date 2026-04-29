---
description: <p/>
layout: schema
name: GetComplianceSummaryByResourceTypeRequest
properties_list:
- description: ''
  name: ResourceTypes
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-compliance-summary-by-resource-type-request-schema.json
slug: config-get-compliance-summary-by-resource-type-request
source_filename: config-get-compliance-summary-by-resource-type-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-summary-by-resource-type-request-schema.json\",\n  \"title\": \"GetComplianceSummaryByResourceTypeRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypes\"\n        },\n        {\n          \"description\": \"<p>Specify one or more resource types to get the number of resources that are compliant and the number that are noncompliant for each resource type.</p> <p>For this request, you can specify an Amazon Web Services resource type such as <code>AWS::EC2::Instance</code>. You can specify that the resource type is an Amazon Web Services account by specifying <code>AWS::::Account</code>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-compliance-summary-by-resource-type-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetComplianceSummaryByResourceTypeRequest
---
