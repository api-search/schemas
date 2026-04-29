---
description: A structure containing information about one error encountered while performing an <a href="https://docs.aws.amazon.com/grafana/latest/APIReference/API_UpdatePermissions.html">UpdatePermissions</a> operation.
layout: schema
name: UpdateError
properties_list:
- description: ''
  name: causedBy
  type: object
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-update-error-schema.json
slug: amazon-managed-grafana-update-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-error-schema.json\",\n  \"title\": \"UpdateError\",\n  \"description\": \"A structure containing information about one error encountered while performing an <a href=\\\"https://docs.aws.amazon.com/grafana/latest/APIReference/API_UpdatePermissions.html\\\">UpdatePermissions</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"causedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateInstruction\"\n        },\n        {\n          \"description\": \"Specifies which permission update caused the error.\"\n        }\n      ]\n    },\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateErrorCodeInteger\"\n        },\n        {\n          \"description\": \"The error code.\"\
  \n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The message for this error.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"causedBy\",\n    \"code\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-error-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: UpdateError
---
