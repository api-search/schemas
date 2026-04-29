---
description: Indicate the availability of the POI Terminal components. The data element is absent if the component is not part of the POI Terminal. State of a POI Terminal.
layout: schema
name: POIStatus
properties_list:
- description: ''
  name: GlobalStatus
  type: object
- description: If security module present.
  name: SecurityOKFlag
  type: boolean
- description: If PED present.
  name: PEDOKFlag
  type: boolean
- description: If card reader device present.
  name: CardReaderOKFlag
  type: boolean
- description: ''
  name: PrinterStatus
  type: object
- description: If communication infrastructure present.
  name: CommunicationOKFlag
  type: boolean
- description: ''
  name: CashHandlingDevice
  type: array
- description: default False.
  name: FraudPreventionFlag
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-poi-status-schema.json
slug: terminal-poi-status
source_filename: terminal-poi-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-status-schema.json\",\n  \"title\": \"POIStatus\",\n  \"description\": \"Indicate the availability of the POI Terminal components. The data element is absent if the component is not part of the POI Terminal. State of a POI Terminal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GlobalStatus\": {\n      \"$ref\": \"#/components/schemas/GlobalStatus\"\n    },\n    \"SecurityOKFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"If security module present.\"\n    },\n    \"PEDOKFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"If PED present.\"\n    },\n    \"CardReaderOKFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"If card reader device present.\"\n    },\n    \"PrinterStatus\": {\n      \"$ref\": \"#/components/schemas/PrinterStatus\"\n    },\n\
  \    \"CommunicationOKFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"If communication infrastructure present.\"\n    },\n    \"CashHandlingDevice\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CashHandlingDevice\"\n      }\n    },\n    \"FraudPreventionFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"default False.\"\n    }\n  },\n  \"required\": [\n    \"GlobalStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: POIStatus
---
