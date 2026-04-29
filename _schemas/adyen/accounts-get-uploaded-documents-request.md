---
description: GetUploadedDocumentsRequest schema from Adyen API
layout: schema
name: GetUploadedDocumentsRequest
properties_list:
- description: The code of the Account Holder for which to retrieve the documents.
  name: accountHolderCode
  type: string
- description: The code of the Bank Account for which to retrieve the documents.
  name: bankAccountUUID
  type: string
- description: The code of the Shareholder for which to retrieve the documents.
  name: shareholderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-get-uploaded-documents-request-schema.json
slug: accounts-get-uploaded-documents-request
source_filename: accounts-get-uploaded-documents-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-get-uploaded-documents-request-schema.json\",\n  \"title\": \"GetUploadedDocumentsRequest\",\n  \"description\": \"GetUploadedDocumentsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder for which to retrieve the documents.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUID\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The code of the Bank Account for which to retrieve the documents.\",\n      \"type\": \"string\"\n    },\n    \"shareholderCode\": {\n      \"description\": \"The code of the Shareholder for which to retrieve the documents.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-get-uploaded-documents-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetUploadedDocumentsRequest
---
