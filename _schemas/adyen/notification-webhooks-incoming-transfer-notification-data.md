---
description: IncomingTransferNotificationData schema from Adyen API
layout: schema
name: IncomingTransferNotificationData
properties_list:
- description: Contains information about the account holder.
  name: accountHolder
  type: object
- description: The amount converted to the balance account's currency, in case the original transaction currency is different. * A _positive_ value means the amount is added to the balance account. * A _negative_ va
  name: amount
  type: object
- description: Contains information about the balance account.
  name: balanceAccount
  type: object
- description: Unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: Contains information about the other party in the transaction.
  name: counterparty
  type: object
- description: Date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.
  name: creationDate
  type: string
- description: Your description for the transfer. If you send a description longer than 140 characters, the text is truncated.
  name: description
  type: string
- description: The ID of the resource.
  name: id
  type: string
- description: Contains the amount and type of modification that triggered the notification. For example, this object contains the amount of a partial cancellation or partial expired authorisation.
  name: modification
  type: object
- description: The amount in the original currency of the transaction. * A _positive_ value means the amount is added to the balance account. * A _negative_ value means the amount is deducted from the balance accoun
  name: originalAmount
  type: object
- description: The ID of the original payment authorisation, refund, or funds transfer request. Use this to trace the original request from the `balancePlatform.payment.created` webhook.
  name: paymentId
  type: string
- description: Contains information about the payment instrument.
  name: paymentInstrument
  type: object
- description: Contains information about the related platform payment.
  name: platformPayment
  type: object
- description: An Adyen-generated unique reference for the transfer.
  name: reference
  type: string
- description: The reference sent to or received from the counterparty. * For outgoing funds, this is the [`referenceForBeneficiary`](https://docs.adyen.com/api-explorer/#/transfers/latest/post/transfers__resParam_r
  name: referenceForBeneficiary
  type: string
- description: The event status. The possible values depend on the `type`. * **Authorised**, **Refused**, or **Error** for type `balancePlatform.payment.created` * **Expired** or **Cancelled** for type `balancePlatf
  name: status
  type: string
- description: Indicates the expected settlement date of this transaction, in ISO 8601 extended format. For example, **2021-08-17T15:34:37+02:00**.
  name: valueDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-incoming-transfer-notification-data-schema.json
slug: notification-webhooks-incoming-transfer-notification-data
source_filename: notification-webhooks-incoming-transfer-notification-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-incoming-transfer-notification-data-schema.json\",\n  \"title\": \"IncomingTransferNotificationData\",\n  \"description\": \"IncomingTransferNotificationData schema from Adyen API\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"description\": \"Contains information about the account holder.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"amount\": {\n      \"description\": \"The amount converted to the balance account's currency, in case the original transaction currency is different.\\n\\n* A _positive_ value means the amount is added to the balance account.\\n\\n * A _negative_ value means the amount is deducted from the balance account. \",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"balanceAccount\": {\n      \"description\":\
  \ \"Contains information about the balance account.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"Unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"counterparty\": {\n      \"description\": \"Contains information about the other party in the transaction.\",\n      \"$ref\": \"#/components/schemas/Counterparty\"\n    },\n    \"creationDate\": {\n      \"description\": \"Date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the transfer. If you send a description longer than 140 characters, the text is truncated.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The ID of the resource.\",\n      \"type\": \"string\"\n    },\n    \"modification\"\
  : {\n      \"description\": \"Contains the amount and type of modification that triggered the notification. For example, this object contains the amount of a partial cancellation or partial expired authorisation.\",\n      \"$ref\": \"#/components/schemas/NotificationModificationData\"\n    },\n    \"originalAmount\": {\n      \"description\": \"The amount in the original currency of the transaction.\\n\\n* A _positive_ value means the amount is added to the balance account.\\n\\n * A _negative_ value means the amount is deducted from the balance account. \",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"paymentId\": {\n      \"description\": \"The ID of the original payment authorisation, refund, or funds transfer request. Use this to trace the original request from the `balancePlatform.payment.created` webhook.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrument\": {\n      \"description\": \"Contains information about the payment instrument.\",\n      \"\
  $ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"platformPayment\": {\n      \"description\": \"Contains information about the related platform payment.\",\n      \"$ref\": \"#/components/schemas/PlatformPayment\"\n    },\n    \"reference\": {\n      \"description\": \"An Adyen-generated unique reference for the transfer.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"referenceForBeneficiary\": {\n      \"description\": \"The reference sent to or received from the counterparty.\\n\\n* For outgoing funds, this is the [`referenceForBeneficiary`](https://docs.adyen.com/api-explorer/#/transfers/latest/post/transfers__resParam_referenceForBeneficiary) from the  [`/transfers`](https://docs.adyen.com/api-explorer/#/transfers/latest/post/transfers) request.\\n\\n * For incoming funds, this is the reference from the sender.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The event status. The\
  \ possible values depend on the `type`.\\n\\n* **Authorised**, **Refused**, or **Error** for type `balancePlatform.payment.created`\\n\\n * **Expired** or **Cancelled** for type `balancePlatform.payment.updated`\\n\\n* **PendingIncomingTransfer** for type `balancePlatform.incomingTransfer.created` \\n\\n* **Refunded** or **IncomingTransfer** for type `balancePlatform.incomingTransfer.updated`\\n\\n * **Captured** or **OutgoingTransfer** for type `balancePlatform.outgoingTransfer.created`\\n\\n* **TransferConfirmed**, **TransferSentOut**, or **TransferFailed** for type `balancePlatform.outgoingTransfer.updated`\\n\\n  \",\n      \"type\": \"string\"\n    },\n    \"valueDate\": {\n      \"description\": \"Indicates the expected settlement date of this transaction, in ISO 8601 extended format. For example, **2021-08-17T15:34:37+02:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"counterparty\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-incoming-transfer-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: IncomingTransferNotificationData
---
