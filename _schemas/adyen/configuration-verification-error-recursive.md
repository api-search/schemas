---
description: VerificationError-recursive schema from Adyen API
layout: schema
name: VerificationError-recursive
properties_list:
- description: Contains the capabilities that the verification error applies to.
  name: capabilities
  type: array
- description: The verification error code.
  name: code
  type: string
- description: A description of the error.
  name: message
  type: string
- description: 'The type of error. Possible values: **invalidInput**, **dataMissing**.'
  name: type
  type: string
- description: Contains the actions that you can take to resolve the verification error.
  name: remediatingActions
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-verification-error-recursive-schema.json
slug: configuration-verification-error-recursive
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-verification-error-recursive-schema.json\",\n  \"title\": \"VerificationError-recursive\",\n  \"description\": \"VerificationError-recursive schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"description\": \"Contains the capabilities that the verification error applies to.\",\n      \"items\": {\n        \"enum\": [\n          \"acceptExternalFunding\",\n          \"acceptPspFunding\",\n          \"acceptTransactionInRestrictedCountries\",\n          \"acceptTransactionInRestrictedCountriesCommercial\",\n          \"acceptTransactionInRestrictedCountriesConsumer\",\n          \"acceptTransactionInRestrictedIndustries\",\n          \"acceptTransactionInRestrictedIndustriesCommercial\",\n          \"acceptTransactionInRestrictedIndustriesConsumer\"\
  ,\n          \"acquiring\",\n          \"atmWithdrawal\",\n          \"atmWithdrawalCommercial\",\n          \"atmWithdrawalConsumer\",\n          \"atmWithdrawalInRestrictedCountries\",\n          \"atmWithdrawalInRestrictedCountriesCommercial\",\n          \"atmWithdrawalInRestrictedCountriesConsumer\",\n          \"authorisedPaymentInstrumentUser\",\n          \"getGrantOffers\",\n          \"issueBankAccount\",\n          \"issueCard\",\n          \"issueCardCommercial\",\n          \"issueCardConsumer\",\n          \"localAcceptance\",\n          \"payout\",\n          \"payoutToTransferInstrument\",\n          \"processing\",\n          \"receiveFromBalanceAccount\",\n          \"receiveFromPlatformPayments\",\n          \"receiveFromThirdParty\",\n          \"receiveFromTransferInstrument\",\n          \"receiveGrants\",\n          \"receivePayments\",\n          \"sendToBalanceAccount\",\n          \"sendToThirdParty\",\n          \"sendToTransferInstrument\",\n          \"thirdPartyFunding\"\
  ,\n          \"useCard\",\n          \"useCardCommercial\",\n          \"useCardConsumer\",\n          \"useCardInRestrictedCountries\",\n          \"useCardInRestrictedCountriesCommercial\",\n          \"useCardInRestrictedCountriesConsumer\",\n          \"useCardInRestrictedIndustries\",\n          \"useCardInRestrictedIndustriesCommercial\",\n          \"useCardInRestrictedIndustriesConsumer\",\n          \"withdrawFromAtm\",\n          \"withdrawFromAtmCommercial\",\n          \"withdrawFromAtmConsumer\",\n          \"withdrawFromAtmInRestrictedCountries\",\n          \"withdrawFromAtmInRestrictedCountriesCommercial\",\n          \"withdrawFromAtmInRestrictedCountriesConsumer\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"code\": {\n      \"description\": \"The verification error code.\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"A description of the error.\",\n      \"type\": \"string\"\n    },\n\
  \    \"type\": {\n      \"description\": \"The type of error.\\n\\n Possible values: **invalidInput**, **dataMissing**.\",\n      \"enum\": [\n        \"dataMissing\",\n        \"invalidInput\",\n        \"pendingStatus\"\n      ],\n      \"type\": \"string\"\n    },\n    \"remediatingActions\": {\n      \"description\": \"Contains the actions that you can take to resolve the verification error.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RemediatingAction\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": []\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-verification-error-recursive-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: VerificationError-recursive
---
