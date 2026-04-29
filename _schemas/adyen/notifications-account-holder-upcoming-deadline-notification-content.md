---
description: AccountHolderUpcomingDeadlineNotificationContent schema from Adyen API
layout: schema
name: AccountHolderUpcomingDeadlineNotificationContent
properties_list:
- description: The code of the account holder whom the event refers to.
  name: accountHolderCode
  type: string
- description: The event name that will be trigger if no action is taken.
  name: event
  type: string
- description: The execution date scheduled for the event.
  name: executionDate
  type: string
- description: The reason that leads to scheduling of the event.
  name: reason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-upcoming-deadline-notification-content-schema.json
slug: notifications-account-holder-upcoming-deadline-notification-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-upcoming-deadline-notification-content-schema.json\",\n  \"title\": \"AccountHolderUpcomingDeadlineNotificationContent\",\n  \"description\": \"AccountHolderUpcomingDeadlineNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder whom the event refers to.\",\n      \"type\": \"string\"\n    },\n    \"event\": {\n      \"description\": \"The event name that will be trigger if no action is taken.\",\n      \"enum\": [\n        \"AccessPii\",\n        \"ApiTierUpdate\",\n        \"CloseAccount\",\n        \"CloseStores\",\n        \"DeleteBalanceAccounts\",\n        \"DeleteBankAccounts\",\n        \"DeleteLegalArrangements\",\n        \"DeleteLiableBankAccount\",\n \
  \       \"DeletePayoutMethods\",\n        \"DeleteShareholders\",\n        \"DeleteSignatories\",\n        \"InactivateAccount\",\n        \"KYCDeadlineExtension\",\n        \"MigrateAccountToBP\",\n        \"RecalculateAccountStatusAndProcessingTier\",\n        \"RefundNotPaidOutTransfers\",\n        \"ResolveEvents\",\n        \"SaveAccountHolder\",\n        \"SaveKYCCheckStatus\",\n        \"SavePEPChecks\",\n        \"SuspendAccount\",\n        \"UnSuspendAccount\",\n        \"UpdateAccountHolderState\",\n        \"Verification\"\n      ],\n      \"type\": \"string\"\n    },\n    \"executionDate\": {\n      \"description\": \"The execution date scheduled for the event.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"The reason that leads to scheduling of the event.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-upcoming-deadline-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderUpcomingDeadlineNotificationContent
---
