---
description: It conveys Information related to the session (period between a Login and the following Logout) to process. Content of the Login Request message.
layout: schema
name: LoginRequest
properties_list:
- description: Date and Time.
  name: DateTime
  type: string
- description: ''
  name: SaleSoftware
  type: object
- description: ''
  name: SaleTerminalData
  type: object
- description: The POI does not realise the transaction with the Acquirer.
  name: TrainingModeFlag
  type: boolean
- description: Default value for Device type displays.
  name: OperatorLanguage
  type: string
- description: '4 conditions to send it: a) the Sale System wants the POI log it in the transaction log b) because of reconciliation.'
  name: OperatorID
  type: string
- description: Same as OperatorID.
  name: ShiftNumber
  type: string
- description: ''
  name: TokenRequestedType
  type: object
- description: ''
  name: CustomerOrderReq
  type: object
- description: If the login involve a POI Terminal and not the first Login to the POI System.
  name: POISerialNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-login-request-schema.json
slug: terminal-login-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-login-request-schema.json\",\n  \"title\": \"LoginRequest\",\n  \"description\": \"It conveys Information related to the session (period between a Login and the following Logout) to process. Content of the Login Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and Time.\"\n    },\n    \"SaleSoftware\": {\n      \"$ref\": \"#/components/schemas/SaleSoftware\"\n    },\n    \"SaleTerminalData\": {\n      \"$ref\": \"#/components/schemas/SaleTerminalData\"\n    },\n    \"TrainingModeFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"The POI does not realise the transaction with the Acquirer.\"\n    },\n    \"OperatorLanguage\": {\n    \
  \  \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"Default value for Device type displays.\"\n    },\n    \"OperatorID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"4 conditions to send it: a) the Sale System wants the POI log it in the transaction log b) because of reconciliation.\"\n    },\n    \"ShiftNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Same as OperatorID.\"\n    },\n    \"TokenRequestedType\": {\n      \"$ref\": \"#/components/schemas/TokenRequestedType\"\n    },\n    \"CustomerOrderReq\": {\n      \"$ref\": \"#/components/schemas/CustomerOrderReq\"\n    },\n    \"POISerialNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If the login involve a POI Terminal and not the first Login to the POI System.\"\n    }\n  },\n  \"required\": [\n    \"DateTime\",\n    \"SaleSoftware\",\n    \"OperatorLanguage\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-login-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoginRequest
---
