---
description: DefendDisputeRequest schema from Adyen API
layout: schema
name: DefendDisputeRequest
properties_list:
- description: The defense reason code that was selected to defend this dispute.
  name: defenseReasonCode
  type: string
- description: The PSP reference assigned to the dispute.
  name: disputePspReference
  type: string
- description: The merchant account identifier, for which you want to process the dispute transaction.
  name: merchantAccountCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-defend-dispute-request-schema.json
slug: disputes-defend-dispute-request
source_filename: disputes-defend-dispute-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defend-dispute-request-schema.json\",\n  \"title\": \"DefendDisputeRequest\",\n  \"description\": \"DefendDisputeRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defenseReasonCode\": {\n      \"description\": \"The defense reason code that was selected to defend this dispute.\",\n      \"type\": \"string\"\n    },\n    \"disputePspReference\": {\n      \"description\": \"The PSP reference assigned to the dispute.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The merchant account identifier, for which you want to process the dispute transaction.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccountCode\",\n    \"disputePspReference\",\n    \"defenseReasonCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defend-dispute-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DefendDisputeRequest
---
