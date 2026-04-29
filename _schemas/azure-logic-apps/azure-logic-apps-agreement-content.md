---
description: The integration account agreement content.
layout: schema
name: AgreementContent
properties_list:
- description: The AS2 agreement content.
  name: aS2
  type: object
- description: The EDIFACT agreement content.
  name: edifact
  type: object
- description: The X12 agreement content.
  name: x12
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-agreement-content-schema.json
slug: azure-logic-apps-agreement-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-agreement-content-schema.json\",\n  \"title\": \"AgreementContent\",\n  \"description\": \"The integration account agreement content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aS2\": {\n      \"$ref\": \"#/definitions/AS2AgreementContent\",\n      \"description\": \"The AS2 agreement content.\"\n    },\n    \"edifact\": {\n      \"$ref\": \"#/definitions/EdifactAgreementContent\",\n      \"description\": \"The EDIFACT agreement content.\"\n    },\n    \"x12\": {\n      \"$ref\": \"#/definitions/X12AgreementContent\",\n      \"description\": \"The X12 agreement content.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-agreement-content-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AgreementContent
---
