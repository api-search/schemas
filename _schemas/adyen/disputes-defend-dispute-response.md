---
description: DefendDisputeResponse schema from Adyen API
layout: schema
name: DefendDisputeResponse
properties_list:
- description: The result of the dispute service.
  name: disputeServiceResult
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-defend-dispute-response-schema.json
slug: disputes-defend-dispute-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defend-dispute-response-schema.json\",\n  \"title\": \"DefendDisputeResponse\",\n  \"description\": \"DefendDisputeResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disputeServiceResult\": {\n      \"description\": \"The result of the dispute service.\",\n      \"$ref\": \"#/components/schemas/DisputeServiceResult\"\n    }\n  },\n  \"required\": [\n    \"disputeServiceResult\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defend-dispute-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DefendDisputeResponse
---
