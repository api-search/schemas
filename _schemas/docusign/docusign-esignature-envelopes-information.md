---
description: Contains information about the envelopes returned by a list request, including the result set and pagination details.
layout: schema
name: EnvelopesInformation
properties_list:
- description: The list of envelopes matching the query.
  name: envelopes
  type: array
- description: The number of results in the current set.
  name: resultSetSize
  type: string
- description: The total number of envelopes matching the query.
  name: totalSetSize
  type: string
- description: The starting index position of the current result set.
  name: startPosition
  type: string
- description: The ending index position of the current result set.
  name: endPosition
  type: string
- description: URI for the next page of results.
  name: nextUri
  type: string
- description: URI for the previous page of results.
  name: previousUri
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelopes-information-schema.json
slug: docusign-esignature-envelopes-information
source_filename: docusign-esignature-envelopes-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopesInformation\",\n  \"type\": \"object\",\n  \"description\": \"Contains information about the envelopes returned by a list request, including the result set and pagination details.\",\n  \"properties\": {\n    \"envelopes\": {\n      \"type\": \"array\",\n      \"description\": \"The list of envelopes matching the query.\"\n    },\n    \"resultSetSize\": {\n      \"type\": \"string\",\n      \"description\": \"The number of results in the current set.\"\n    },\n    \"totalSetSize\": {\n      \"type\": \"string\",\n      \"description\": \"The total number of envelopes matching the query.\"\n    },\n    \"startPosition\": {\n      \"type\": \"string\",\n      \"description\": \"The starting index position of the current result set.\"\n    },\n    \"endPosition\": {\n      \"type\": \"string\",\n      \"description\": \"The ending index position of the current result set.\"\n    },\n\
  \    \"nextUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI for the next page of results.\"\n    },\n    \"previousUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI for the previous page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelopes-information-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopesInformation
---
