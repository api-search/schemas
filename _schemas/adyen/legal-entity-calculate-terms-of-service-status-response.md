---
description: CalculateTermsOfServiceStatusResponse schema from Adyen API
layout: schema
name: CalculateTermsOfServiceStatusResponse
properties_list:
- description: The type of Terms of Service that the legal entity needs to accept. If empty, no Terms of Service needs to be accepted.
  name: termsOfServiceTypes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-calculate-terms-of-service-status-response-schema.json
slug: legal-entity-calculate-terms-of-service-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-calculate-terms-of-service-status-response-schema.json\",\n  \"title\": \"CalculateTermsOfServiceStatusResponse\",\n  \"description\": \"CalculateTermsOfServiceStatusResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"termsOfServiceTypes\": {\n      \"description\": \"The type of Terms of Service that the legal entity needs to accept. If empty, no Terms of Service needs to be accepted.\",\n      \"items\": {\n        \"enum\": [\n          \"adyenAccount\",\n          \"adyenCapital\",\n          \"adyenCard\",\n          \"adyenForPlatformsAdvanced\",\n          \"adyenForPlatformsManage\",\n          \"adyenFranchisee\",\n          \"adyenIssuing\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-calculate-terms-of-service-status-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CalculateTermsOfServiceStatusResponse
---
