---
description: TestOutput schema from Adyen API
layout: schema
name: TestOutput
properties_list:
- description: Unique identifier of the merchant account that the notification is about.
  name: merchantId
  type: string
- description: 'The response your server returned for the test webhook. Your server must respond with **[accepted]** for the test webhook to be successful (`data.status`: **success**). Find out more about [accepting '
  name: output
  type: string
- description: The [body of the notification webhook](https://docs.adyen.com/development-resources/webhooks/understand-notifications#notification-structure) that was sent to your server.
  name: requestSent
  type: string
- description: The HTTP response code for your server's response to the test webhook. You can use the value of this field together with the the [`output`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/p
  name: responseCode
  type: string
- description: The time between sending the test webhook and receiving the response from your server. You can use it as an indication of how long your server takes to process a webhook notification. Measured in mill
  name: responseTime
  type: string
- description: 'The status of the test request. Possible values are: * **success**, if `data.output`: **[accepted]** and `data.responseCode`: **200**. * **failed**, in all other cases. You can use the value of the [`'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-test-output-schema.json
slug: management-test-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-test-output-schema.json\",\n  \"title\": \"TestOutput\",\n  \"description\": \"TestOutput schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantId\": {\n      \"description\": \"Unique identifier of the merchant account that the notification is about.\",\n      \"type\": \"string\"\n    },\n    \"output\": {\n      \"description\": \"The response your server returned for the test webhook.\\n\\nYour server must respond with **[accepted]** for the test webhook to be successful (`data.status`: **success**). Find out more about [accepting notifications](https://docs.adyen.com/development-resources/webhooks#accept-notifications)\\n\\nYou can use the value of this field together with the [`responseCode`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/post/merchants/{merchantId}/webhooks/{id}/test__resParam_data-responseCode)\
  \ value to troubleshoot unsuccessful test webhooks.\",\n      \"type\": \"string\"\n    },\n    \"requestSent\": {\n      \"description\": \"The [body of the notification webhook](https://docs.adyen.com/development-resources/webhooks/understand-notifications#notification-structure) that was sent to your server.\",\n      \"type\": \"string\"\n    },\n    \"responseCode\": {\n      \"description\": \"The HTTP response code for your server's response to the test webhook.\\n\\nYou can use the value of this field together with the the [`output`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/post/merchants/{merchantId}/webhooks/{id}/test__resParam_data-output) field value to troubleshoot failed test webhooks.\",\n      \"example\": \"200\",\n      \"type\": \"string\"\n    },\n    \"responseTime\": {\n      \"description\": \"The time between sending the test webhook and receiving the response from your server. You can use it as an indication of how long your server takes to process\
  \ a webhook notification. Measured in milliseconds, for example **304 ms**.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the test request. Possible values are:\\n* **success**, if `data.output`: **[accepted]** and `data.responseCode`: **200**.\\n* **failed**, in all other cases.\\n\\nYou can use the value of the [`output`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/post/merchants/{merchantId}/webhooks/{id}/test__resParam_data-output) field together with the [`responseCode`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/post/merchants/{merchantId}/webhooks/{id}/test__resParam_data-responseCode) value to troubleshoot failed test webhooks.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-test-output-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TestOutput
---
