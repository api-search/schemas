---
description: TermsOfServiceAcceptanceInfo schema from Adyen API
layout: schema
name: TermsOfServiceAcceptanceInfo
properties_list:
- description: The unique identifier of the user that accepted the Terms of Service.
  name: acceptedBy
  type: string
- description: The unique identifier of the legal entity for which the Terms of Service are accepted.
  name: acceptedFor
  type: string
- description: The date when the Terms of Service were accepted.
  name: createdAt
  type: string
- description: An Adyen-generated reference for the accepted Terms of Service.
  name: id
  type: string
- description: 'The type of Terms of Service. Possible values: * **adyenForPlatformsManage** * **adyenIssuing** * **adyenForPlatformsAdvanced** * **adyenCapital** * **adyenAccount** * **adyenCard** * **adyenFranchise'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-terms-of-service-acceptance-info-schema.json
slug: legal-entity-terms-of-service-acceptance-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-terms-of-service-acceptance-info-schema.json\",\n  \"title\": \"TermsOfServiceAcceptanceInfo\",\n  \"description\": \"TermsOfServiceAcceptanceInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptedBy\": {\n      \"description\": \"The unique identifier of the user that accepted the Terms of Service.\",\n      \"type\": \"string\"\n    },\n    \"acceptedFor\": {\n      \"description\": \"The unique identifier of the legal entity for which the Terms of Service are accepted.\",\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"description\": \"The date when the Terms of Service were accepted.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"An Adyen-generated reference for the accepted\
  \ Terms of Service.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of Terms of Service.\\n\\nPossible values:\\n*  **adyenForPlatformsManage**\\n*  **adyenIssuing**\\n*  **adyenForPlatformsAdvanced**\\n*  **adyenCapital**\\n*  **adyenAccount**\\n*  **adyenCard**\\n*  **adyenFranchisee**\\n\\n\",\n      \"enum\": [\n        \"adyenAccount\",\n        \"adyenCapital\",\n        \"adyenCard\",\n        \"adyenForPlatformsAdvanced\",\n        \"adyenForPlatformsManage\",\n        \"adyenFranchisee\",\n        \"adyenIssuing\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-terms-of-service-acceptance-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TermsOfServiceAcceptanceInfo
---
