---
description: Set of Personally Identifiable Information (PII) associated with a given client.
layout: schema
name: BasicProfile
properties_list:
- description: First name of the client. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client.
  name: firstName
  type: string
- description: Middle name 1 of the client. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: middleName1
  type: string
- description: Middle name 2 of the client. Not applicable for Add-on client. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: middleName2
  type: string
- description: Last name of the client. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client.
  name: lastName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-basic-profile-schema.json
slug: mastercard-card-issuance-basic-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BasicProfile\",\n  \"type\": \"object\",\n  \"description\": \"Set of Personally Identifiable Information (PII) associated with a given client.\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the client. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client.\"\n    },\n    \"middleName1\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name 1 of the client. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"middleName2\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name 2 of the client. Not applicable for Add-on client. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Last name of the client. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-basic-profile-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BasicProfile
---
