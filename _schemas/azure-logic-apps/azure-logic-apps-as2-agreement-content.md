---
description: The integration account AS2 agreement content.
layout: schema
name: AS2AgreementContent
properties_list:
- description: The AS2 one-way receive agreement.
  name: receiveAgreement
  type: object
- description: The AS2 one-way send agreement.
  name: sendAgreement
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-agreement-content-schema.json
slug: azure-logic-apps-as2-agreement-content
source_filename: azure-logic-apps-as2-agreement-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-agreement-content-schema.json\",\n  \"title\": \"AS2AgreementContent\",\n  \"description\": \"The integration account AS2 agreement content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"receiveAgreement\": {\n      \"$ref\": \"#/definitions/AS2OneWayAgreement\",\n      \"description\": \"The AS2 one-way receive agreement.\"\n    },\n    \"sendAgreement\": {\n      \"$ref\": \"#/definitions/AS2OneWayAgreement\",\n      \"description\": \"The AS2 one-way send agreement.\"\n    }\n  },\n  \"required\": [\n    \"receiveAgreement\",\n    \"sendAgreement\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-agreement-content-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2AgreementContent
---
