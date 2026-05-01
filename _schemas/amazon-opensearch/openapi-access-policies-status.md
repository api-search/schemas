---
description: The configured access rules for the domain's document and search endpoints, and the current status of those rules.
layout: schema
name: AccessPoliciesStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-access-policies-status-schema.json
slug: openapi-access-policies-status
source_filename: openapi-access-policies-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-access-policies-status-schema.json\",\n  \"title\": \"AccessPoliciesStatus\",\n  \"description\": \"The configured access rules for the domain's document and search endpoints, and the current status of those rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"The access policy configured for the Elasticsearch domain. Access policies may be resource-based, IP-based, or IAM-based. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-access-policies\\\" target=\\\"_blank\\\"> Configuring Access Policies</a>for more information.\"\n        }\n\
  \      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionStatus\"\n        },\n        {\n          \"description\": \"The status of the access policy for the Elasticsearch domain. See <code>OptionStatus</code> for the status information that's included. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Options\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-access-policies-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: AccessPoliciesStatus
---
