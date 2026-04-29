---
description: CustomNotification schema from Adyen API
layout: schema
name: CustomNotification
properties_list:
- description: The amount of the payment that the notification is about. Set the value in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: amount
  type: object
- description: 'The event that caused the notification to be sent.Currently supported values: * **AUTHORISATION** * **CANCELLATION** * **REFUND** * **CAPTURE** * **REPORT_AVAILABLE** * **CHARGEBACK** * **REQUEST_FOR_'
  name: eventCode
  type: string
- description: 'The time of the event. Format: [ISO 8601](http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDThh:mm:ssTZD.'
  name: eventDate
  type: string
- description: Your reference for the custom test notification.
  name: merchantReference
  type: string
- description: 'The payment method for the payment that the notification is about. Possible values: * **amex** * **visa** * **mc** * **maestro** * **bcmc** * **paypal** * **sms** * **bankTransfer_NL** * **bankTransfe'
  name: paymentMethod
  type: string
- description: A descripton of what caused the notification.
  name: reason
  type: string
- description: The outcome of the event which the notification is about. Set to either **true** or **false**.
  name: success
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-custom-notification-schema.json
slug: management-custom-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-custom-notification-schema.json\",\n  \"title\": \"CustomNotification\",\n  \"description\": \"CustomNotification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount of the payment that the notification is about. Set the value in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"eventCode\": {\n      \"description\": \"The event that caused the notification to be sent.Currently supported values:\\n* **AUTHORISATION**\\n* **CANCELLATION**\\n* **REFUND**\\n* **CAPTURE**\\n* **REPORT_AVAILABLE**\\n* **CHARGEBACK**\\n* **REQUEST_FOR_INFORMATION**\\n* **NOTIFICATION_OF_CHARGEBACK**\\n* **NOTIFICATIONTEST**\\n* **ORDER_OPENED**\\n* **ORDER_CLOSED**\\\
  n* **CHARGEBACK_REVERSED**\\n* **REFUNDED_REVERSED**\\n* **REFUND_WITH_DATA**\",\n      \"type\": \"string\"\n    },\n    \"eventDate\": {\n      \"description\": \"The time of the event. Format: [ISO 8601](http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDThh:mm:ssTZD.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"description\": \"Your reference for the custom test notification.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethod\": {\n      \"description\": \"The payment method for the payment that the notification is about. Possible values:\\n* **amex**\\n* **visa**\\n* **mc**\\n* **maestro**\\n* **bcmc**\\n* **paypal**\\n * **sms**\\n * **bankTransfer_NL**\\n* **bankTransfer_DE**\\n* **bankTransfer_BE**\\n* **ideal**\\n* **elv**\\n* **sepadirectdebit**\\n\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"A descripton of what caused the notification.\",\n      \"type\": \"string\"\
  \n    },\n    \"success\": {\n      \"description\": \"The outcome of the event which the notification is about. Set to either **true** or **false**. \",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-custom-notification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CustomNotification
---
