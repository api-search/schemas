---
description: GetTermsOfServiceDocumentRequest schema from Adyen API
layout: schema
name: GetTermsOfServiceDocumentRequest
properties_list:
- description: 'The language to be used for the Terms of Service document, specified by the two-letter [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language code. Possible value: **en** for Engl'
  name: language
  type: string
- description: 'The type of Terms of Service. Possible values: * **adyenForPlatformsManage** * **adyenIssuing** * **adyenForPlatformsAdvanced** * **adyenCapital** * **adyenAccount** * **adyenCard** * **adyenFranchise'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-get-terms-of-service-document-request-schema.json
slug: legal-entity-get-terms-of-service-document-request
source_filename: legal-entity-get-terms-of-service-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-get-terms-of-service-document-request-schema.json\",\n  \"title\": \"GetTermsOfServiceDocumentRequest\",\n  \"description\": \"GetTermsOfServiceDocumentRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"description\": \"The language to be used for the Terms of Service document, specified by the two-letter [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language code. Possible value: **en** for English.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of Terms of Service.\\n\\nPossible values:\\n*  **adyenForPlatformsManage**\\n*  **adyenIssuing**\\n*  **adyenForPlatformsAdvanced**\\n*  **adyenCapital**\\n*  **adyenAccount**\\n*  **adyenCard**\\n*  **adyenFranchisee**\\n\\n\",\n    \
  \  \"enum\": [\n        \"adyenAccount\",\n        \"adyenCapital\",\n        \"adyenCard\",\n        \"adyenForPlatformsAdvanced\",\n        \"adyenForPlatformsManage\",\n        \"adyenFranchisee\",\n        \"adyenIssuing\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"language\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-get-terms-of-service-document-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetTermsOfServiceDocumentRequest
---
