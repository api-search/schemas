---
description: Instalment schema from Adyen API
layout: schema
name: Instalment
properties_list:
- description: ''
  name: InstalmentType
  type: object
- description: ''
  name: SequenceNumber
  type: integer
- description: ''
  name: PlanID
  type: string
- description: ''
  name: Period
  type: integer
- description: ''
  name: PeriodUnit
  type: object
- description: ''
  name: FirstPaymentDate
  type: string
- description: ''
  name: TotalNbOfPayments
  type: integer
- description: ''
  name: CumulativeAmount
  type: number
- description: ''
  name: FirstAmount
  type: number
- description: ''
  name: Charges
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-instalment-schema.json
slug: terminal-instalment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-instalment-schema.json\",\n  \"title\": \"Instalment\",\n  \"description\": \"Instalment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstalmentType\": {\n      \"$ref\": \"#/components/schemas/InstalmentType\"\n    },\n    \"SequenceNumber\": {\n      \"type\": \"integer\"\n    },\n    \"PlanID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"Period\": {\n      \"type\": \"integer\"\n    },\n    \"PeriodUnit\": {\n      \"$ref\": \"#/components/schemas/PeriodUnit\"\n    },\n    \"FirstPaymentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"TotalNbOfPayments\": {\n      \"type\": \"integer\"\n    },\n    \"CumulativeAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\"\
  : 0\n    },\n    \"FirstAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"Charges\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-instalment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Instalment
---
