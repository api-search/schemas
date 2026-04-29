---
description: StoredValueIssueResponse schema from Adyen API
layout: schema
name: StoredValueIssueResponse
properties_list:
- description: 'Authorisation code: * When the payment is authorised, this field holds the authorisation code for the payment. * When the payment is not authorised, this field is empty.'
  name: authCode
  type: string
- description: The balance currently on the payment method.
  name: currentBalance
  type: object
- description: The collection that contains the type of the payment method and its specific information if available
  name: paymentMethod
  type: object
- description: Adyen's 16-character string reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.
  name: pspReference
  type: string
- description: If the transaction is refused or an error occurs, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the authorisation response includes `r
  name: refusalReason
  type: string
- description: 'The result of the payment. Possible values: * **Success** – The operation has been completed successfully. * **Refused** – The operation was refused. The reason is given in the `refusalReason` field. '
  name: resultCode
  type: string
- description: Raw refusal reason received from the third party, where available
  name: thirdPartyRefusalReason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/stored-value-stored-value-issue-response-schema.json
slug: stored-value-stored-value-issue-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/stored-value-stored-value-issue-response-schema.json\",\n  \"title\": \"StoredValueIssueResponse\",\n  \"description\": \"StoredValueIssueResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authCode\": {\n      \"description\": \"Authorisation code:\\n* When the payment is authorised, this field holds the authorisation code for the payment.\\n* When the payment is not authorised, this field is empty.\",\n      \"type\": \"string\"\n    },\n    \"currentBalance\": {\n      \"description\": \"The balance currently on the payment method.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"paymentMethod\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The collection that contains the type of the payment method\
  \ and its specific information if available\",\n      \"type\": \"object\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character string reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"refusalReason\": {\n      \"description\": \"If the transaction is refused or an error occurs, this field holds Adyen's mapped reason for the refusal or a description of the error.\\n\\nWhen a transaction fails, the authorisation response includes `resultCode` and `refusalReason` values.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result of the payment. Possible values:\\n\\n* **Success** \\u2013 The operation has been completed successfully. \\n* **Refused** \\u2013 The operation was refused. The reason is given in the `refusalReason` field. \\n* **Error** \\u2013 There was an error when the operation\
  \ was processed. The reason is given in the `refusalReason` field. \\n* **NotEnoughBalance** \\u2013 The amount on the payment method is lower than the amount given in the request. Only applicable to balance checks. \\n\",\n      \"enum\": [\n        \"Success\",\n        \"Refused\",\n        \"Error\",\n        \"NotEnoughBalance\"\n      ],\n      \"type\": \"string\"\n    },\n    \"thirdPartyRefusalReason\": {\n      \"description\": \"Raw refusal reason received from the third party, where available\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/stored-value-stored-value-issue-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueIssueResponse
---
