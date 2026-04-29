---
description: UploadDocumentRequest schema from Adyen API
layout: schema
name: UploadDocumentRequest
properties_list:
- description: The content of the document, in Base64-encoded string format. To learn about document requirements, refer to [Verification checks](https://docs.adyen.com/marketplaces-and-platforms/classic/verificatio
  name: documentContent
  type: string
- description: Details of the document being submitted.
  name: documentDetail
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-upload-document-request-schema.json
slug: accounts-upload-document-request
source_filename: accounts-upload-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-upload-document-request-schema.json\",\n  \"title\": \"UploadDocumentRequest\",\n  \"description\": \"UploadDocumentRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentContent\": {\n      \"description\": \"The content of the document, in Base64-encoded string format.\\n\\nTo learn about document requirements, refer to [Verification checks](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks).\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"documentDetail\": {\n      \"description\": \"Details of the document being submitted.\",\n      \"$ref\": \"#/components/schemas/DocumentDetail\"\n    }\n  },\n  \"required\": [\n    \"documentDetail\",\n    \"documentContent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-upload-document-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UploadDocumentRequest
---
