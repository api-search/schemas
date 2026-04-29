---
description: TestWebhookRequest schema from Adyen API
layout: schema
name: TestWebhookRequest
properties_list:
- description: Custom test notification object. Required when the [`types`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/post/companies/{companyId}/webhooks/{webhookId}/test__reqParam_types) list conta
  name: notification
  type: object
- description: 'List of event codes for which to send test notifications. Only the webhook types below are supported. Possible values if webhook `type`: **standard**: * **AUTHORISATION** * **CHARGEBACK_REVERSED** * *'
  name: types
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-test-webhook-request-schema.json
slug: management-test-webhook-request
source_filename: management-test-webhook-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-test-webhook-request-schema.json\",\n  \"title\": \"TestWebhookRequest\",\n  \"description\": \"TestWebhookRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notification\": {\n      \"description\": \"Custom test notification object. Required when the [`types`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/post/companies/{companyId}/webhooks/{webhookId}/test__reqParam_types) list contains **CUSTOM**.\",\n      \"$ref\": \"#/components/schemas/CustomNotification\"\n    },\n    \"types\": {\n      \"description\": \"List of event codes for which to send test notifications. Only the webhook types below are supported. \\n\\nPossible values if webhook `type`: **standard**:\\n\\n* **AUTHORISATION**\\n* **CHARGEBACK_REVERSED**\\n* **ORDER_CLOSED**\\n* **ORDER_OPENED**\\\
  n* **PAIDOUT_REVERSED**\\n* **PAYOUT_THIRDPARTY**\\n* **REFUNDED_REVERSED**\\n* **REFUND_WITH_DATA**\\n* **REPORT_AVAILABLE**\\n* **CUSTOM** - set your custom notification fields in the [`notification`](https://docs.adyen.com/api-explorer/#/ManagementService/v1/post/companies/{companyId}/webhooks/{webhookId}/test__reqParam_notification) object.\\n\\nPossible values if webhook `type`: **banktransfer-notification**:\\n\\n* **PENDING**\\n\\nPossible values if webhook `type`: **report-notification**:\\n\\n* **REPORT_AVAILABLE**\\n\\nPossible values if webhook `type`: **ideal-notification**:\\n\\n* **AUTHORISATION**\\n\\nPossible values if webhook `type`: **pending-notification**:\\n\\n* **PENDING**\\n\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-test-webhook-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TestWebhookRequest
---
