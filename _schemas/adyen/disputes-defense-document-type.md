---
description: DefenseDocumentType schema from Adyen API
layout: schema
name: DefenseDocumentType
properties_list:
- description: When **true**, you've successfully uploaded this type of defense document. When **false**, you haven't uploaded this defense document type.
  name: available
  type: boolean
- description: The document type code of the defense document.
  name: defenseDocumentTypeCode
  type: string
- description: 'Indicates to what extent the defense document is required in the defense process. Possible values: * **Required**: You must supply the document. * **OneOrMore**: You must supply at least one of the do'
  name: requirementLevel
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-defense-document-type-schema.json
slug: disputes-defense-document-type
source_filename: disputes-defense-document-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-document-type-schema.json\",\n  \"title\": \"DefenseDocumentType\",\n  \"description\": \"DefenseDocumentType schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"available\": {\n      \"description\": \"When **true**, you've successfully uploaded this type of defense document. When **false**, you haven't uploaded this defense document type.\",\n      \"type\": \"boolean\"\n    },\n    \"defenseDocumentTypeCode\": {\n      \"description\": \"The document type code of the defense document.\",\n      \"type\": \"string\"\n    },\n    \"requirementLevel\": {\n      \"description\": \"Indicates to what extent the defense document is required in the defense process.\\n\\nPossible values: \\n\\n* **Required**: You must supply the document.\\n\\n * **OneOrMore**: You must supply\
  \ at least one of the documents with this label.\\n\\n* **Optional**: You can choose to supply the document.\\n\\n* **AlternativeRequired**: You must supply a generic defense document. To enable this functionality, contact our Support Team. When enabled, you can supply a generic defense document for all schemes.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"defenseDocumentTypeCode\",\n    \"requirementLevel\",\n    \"available\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-document-type-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DefenseDocumentType
---
