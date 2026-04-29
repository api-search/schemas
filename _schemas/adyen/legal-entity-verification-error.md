---
description: VerificationError schema from Adyen API
layout: schema
name: VerificationError
properties_list:
- description: Contains key-value pairs that specify the actions that the legal entity can do in your platform. The key is a capability required for your integration. For example, **issueCard** for Issuing.The value
  name: capabilities
  type: array
- description: The general error code.
  name: code
  type: string
- description: The general error message.
  name: message
  type: string
- description: An object containing possible solutions to fix a verification error.
  name: remediatingActions
  type: array
- description: An array containing more granular information about the cause of the verification error.
  name: subErrors
  type: array
- description: The type of error.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-verification-error-schema.json
slug: legal-entity-verification-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-verification-error-schema.json\",\n  \"title\": \"VerificationError\",\n  \"description\": \"VerificationError schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"description\": \"Contains key-value pairs that specify the actions that the legal entity can do in your platform. The key is a capability required for your integration. For example, **issueCard** for Issuing.The value is an object containing the settings for the capability.\",\n      \"items\": {\n        \"enum\": [\n          \"acceptExternalFunding\",\n          \"acceptPspFunding\",\n          \"acceptTransactionInRestrictedCountries\",\n          \"acceptTransactionInRestrictedCountriesCommercial\",\n          \"acceptTransactionInRestrictedCountriesConsumer\",\n          \"acceptTransactionInRestrictedIndustries\"\
  ,\n          \"acceptTransactionInRestrictedIndustriesCommercial\",\n          \"acceptTransactionInRestrictedIndustriesConsumer\",\n          \"acquiring\",\n          \"atmWithdrawal\",\n          \"atmWithdrawalCommercial\",\n          \"atmWithdrawalConsumer\",\n          \"atmWithdrawalInRestrictedCountries\",\n          \"atmWithdrawalInRestrictedCountriesCommercial\",\n          \"atmWithdrawalInRestrictedCountriesConsumer\",\n          \"authorisedPaymentInstrumentUser\",\n          \"getGrantOffers\",\n          \"issueBankAccount\",\n          \"issueCard\",\n          \"issueCardCommercial\",\n          \"issueCardConsumer\",\n          \"localAcceptance\",\n          \"payout\",\n          \"payoutToTransferInstrument\",\n          \"processing\",\n          \"receiveFromBalanceAccount\",\n          \"receiveFromPlatformPayments\",\n          \"receiveFromThirdParty\",\n          \"receiveFromTransferInstrument\",\n          \"receiveGrants\",\n          \"receivePayments\"\
  ,\n          \"sendToBalanceAccount\",\n          \"sendToThirdParty\",\n          \"sendToTransferInstrument\",\n          \"thirdPartyFunding\",\n          \"useCard\",\n          \"useCardCommercial\",\n          \"useCardConsumer\",\n          \"useCardInRestrictedCountries\",\n          \"useCardInRestrictedCountriesCommercial\",\n          \"useCardInRestrictedCountriesConsumer\",\n          \"useCardInRestrictedIndustries\",\n          \"useCardInRestrictedIndustriesCommercial\",\n          \"useCardInRestrictedIndustriesConsumer\",\n          \"withdrawFromAtm\",\n          \"withdrawFromAtmCommercial\",\n          \"withdrawFromAtmConsumer\",\n          \"withdrawFromAtmInRestrictedCountries\",\n          \"withdrawFromAtmInRestrictedCountriesCommercial\",\n          \"withdrawFromAtmInRestrictedCountriesConsumer\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"code\": {\n      \"description\": \"The general error code.\",\n     \
  \ \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"The general error message.\",\n      \"type\": \"string\"\n    },\n    \"remediatingActions\": {\n      \"description\": \"An object containing possible solutions to fix a verification error.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RemediatingAction\"\n      },\n      \"type\": \"array\"\n    },\n    \"subErrors\": {\n      \"description\": \"An array containing more granular information about the cause of the verification error.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VerificationError-recursive\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"The type of error.\",\n      \"enum\": [\n        \"dataMissing\",\n        \"dataReview\",\n        \"invalidInput\",\n        \"pendingStatus\",\n        \"rejected\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-verification-error-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: VerificationError
---
