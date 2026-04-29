---
description: VerificationDeadline schema from Adyen API
layout: schema
name: VerificationDeadline
properties_list:
- description: The list of capabilities that will be disallowed if information is not reviewed by the time of the deadline
  name: capabilities
  type: array
- description: The unique identifiers of the bank account(s) that the deadline applies to
  name: entityIds
  type: array
- description: The date that verification is due by before capabilities are disallowed.
  name: expiresAt
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-verification-deadline-schema.json
slug: legal-entity-verification-deadline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-verification-deadline-schema.json\",\n  \"title\": \"VerificationDeadline\",\n  \"description\": \"VerificationDeadline schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"description\": \"The list of capabilities that will be disallowed if information is not reviewed by the time of the deadline\",\n      \"items\": {\n        \"enum\": [\n          \"acceptExternalFunding\",\n          \"acceptPspFunding\",\n          \"acceptTransactionInRestrictedCountries\",\n          \"acceptTransactionInRestrictedCountriesCommercial\",\n          \"acceptTransactionInRestrictedCountriesConsumer\",\n          \"acceptTransactionInRestrictedIndustries\",\n          \"acceptTransactionInRestrictedIndustriesCommercial\",\n          \"acceptTransactionInRestrictedIndustriesConsumer\"\
  ,\n          \"acquiring\",\n          \"atmWithdrawal\",\n          \"atmWithdrawalCommercial\",\n          \"atmWithdrawalConsumer\",\n          \"atmWithdrawalInRestrictedCountries\",\n          \"atmWithdrawalInRestrictedCountriesCommercial\",\n          \"atmWithdrawalInRestrictedCountriesConsumer\",\n          \"authorisedPaymentInstrumentUser\",\n          \"getGrantOffers\",\n          \"issueBankAccount\",\n          \"issueCard\",\n          \"issueCardCommercial\",\n          \"issueCardConsumer\",\n          \"localAcceptance\",\n          \"payout\",\n          \"payoutToTransferInstrument\",\n          \"processing\",\n          \"receiveFromBalanceAccount\",\n          \"receiveFromPlatformPayments\",\n          \"receiveFromThirdParty\",\n          \"receiveFromTransferInstrument\",\n          \"receiveGrants\",\n          \"receivePayments\",\n          \"sendToBalanceAccount\",\n          \"sendToThirdParty\",\n          \"sendToTransferInstrument\",\n          \"thirdPartyFunding\"\
  ,\n          \"useCard\",\n          \"useCardCommercial\",\n          \"useCardConsumer\",\n          \"useCardInRestrictedCountries\",\n          \"useCardInRestrictedCountriesCommercial\",\n          \"useCardInRestrictedCountriesConsumer\",\n          \"useCardInRestrictedIndustries\",\n          \"useCardInRestrictedIndustriesCommercial\",\n          \"useCardInRestrictedIndustriesConsumer\",\n          \"withdrawFromAtm\",\n          \"withdrawFromAtmCommercial\",\n          \"withdrawFromAtmConsumer\",\n          \"withdrawFromAtmInRestrictedCountries\",\n          \"withdrawFromAtmInRestrictedCountriesCommercial\",\n          \"withdrawFromAtmInRestrictedCountriesConsumer\"\n        ],\n        \"type\": \"string\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"entityIds\": {\n      \"description\": \"The unique identifiers of the bank account(s) that the deadline applies to\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"\
  readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"expiresAt\": {\n      \"description\": \"The date that verification is due by before capabilities are disallowed.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"expiresAt\",\n    \"capabilities\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-verification-deadline-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: VerificationDeadline
---
