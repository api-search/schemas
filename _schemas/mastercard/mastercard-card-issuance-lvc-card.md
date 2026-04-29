---
description: LVC Card information
layout: schema
name: LVCCard
properties_list:
- description: It is the limit set for each transaction. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card.
  name: perTransactionLimit
  type: string
- description: It is the maximum transaction limit configured for the client. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card.
  name: totalTransactionLimit
  type: string
- description: Number of times the card can be used in a configured duration. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card.
  name: velocity
  type: string
- description: Card validity duration after which the card gets expired. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card. <BR/> Must be expressed in ISO 8601
  name: validity
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-lvc-card-schema.json
slug: mastercard-card-issuance-lvc-card
source_filename: mastercard-card-issuance-lvc-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LVCCard\",\n  \"type\": \"object\",\n  \"description\": \"LVC Card information\",\n  \"properties\": {\n    \"perTransactionLimit\": {\n      \"type\": \"string\",\n      \"description\": \"It is the limit set for each transaction. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card.\"\n    },\n    \"totalTransactionLimit\": {\n      \"type\": \"string\",\n      \"description\": \"It is the maximum transaction limit configured for the client. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card.\"\n    },\n    \"velocity\": {\n      \"type\": \"string\",\n      \"description\": \"Number of times the card can be used in a configured duration. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card.\"\n    },\n    \"validity\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Card validity duration after which the card gets expired. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required while requesting for LVC card. <BR/> Must be expressed in ISO 8601 Durations format: <BR/> Format - P(n)Y(n)M(n)DT(n)H(n)M(n)S <BR/> <BR/> Where: <BR/>\\n* (n) is replaced by the value for each of the date and time elements that follow the (n). <BR/>\\n* P is the duration designator (referred to as \\\"period\\\"), and is always placed at the beginning of the duration. <BR/>\\n* Y is the year designator that follows the value for the number of years. <BR/>\\n* M is the month designator that follows the value for the number of months. <BR/>\\n* W is the week designator that follows the value for the number of weeks. <BR/>\\n* D is the day designator that follows the value for the number of days. <BR/>\\n* T is the time designator that precedes the time components. <BR/>\\n* H is the hour designator that follows\
  \ the value for the number of hours. <BR/>\\n* M is the minute designator that follows the value for the number of minutes. <BR/> * S is the second designator that follows the value for the number of seconds. <BR/> Maximum validity period: 3 Years\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-lvc-card-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: LVCCard
---
