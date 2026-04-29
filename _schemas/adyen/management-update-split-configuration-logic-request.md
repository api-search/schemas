---
description: UpdateSplitConfigurationLogicRequest schema from Adyen API
layout: schema
name: UpdateSplitConfigurationLogicRequest
properties_list:
- description: 'Specifies the logic to apply when booking the transaction fees. Should be combined with adyenFees. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.'
  name: acquiringFees
  type: string
- description: Contains the logic used to calculate your user's commission, booked directly to their balance account.
  name: additionalCommission
  type: object
- description: 'Specifies the logic to apply when booking the transaction fees. Should be combined with schemeFee, interchange & adyenMarkup. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAccoun'
  name: adyenCommission
  type: string
- description: 'Specifies the logic to apply when booking the transaction fees. Should be combined with acquiringFees. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.'
  name: adyenFees
  type: string
- description: 'Specifies the logic to apply when booking the transaction fees. Should be combined with schemeFee, adyenCommission & interchange. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAc'
  name: adyenMarkup
  type: string
- description: 'Specifies the logic to apply when booking the chargeback amount. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**, **deductAccordingToSplitRatio**.'
  name: chargeback
  type: string
- description: 'Specifies the logic to apply when allocating the chargeback costs. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**'
  name: chargebackCostAllocation
  type: string
- description: Contains the logic used to the calculate your platform's commission, booked to your liable balance account.
  name: commission
  type: object
- description: 'Specifies the logic to apply when booking the transaction fees. Should be combined with schemeFee, adyenCommission & adyenMarkup. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAc'
  name: interchange
  type: string
- description: 'Specifies the logic to apply when booking the transaction fees. Cannot be combined with other fees. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.'
  name: paymentFee
  type: string
- description: 'Specifies the logic to apply when booking the amount left over after currency conversion. Possible values: **addToLiableAccount**, **addToOneBalanceAccount**.'
  name: remainder
  type: string
- description: 'Specifies the logic to apply when booking the transaction fees. Should be combined with interchange, adyenCommission & adyenMarkup. Possible values: **deductFromLiableAccount**, **deductFromOneBalance'
  name: schemeFee
  type: string
- description: Unique identifier of the split logic that is applied when the split configuration conditions are met.
  name: splitLogicId
  type: string
- description: 'Specifies the logic to apply when booking the surcharge amount. Possible values: **addToLiableAccount**, **addToOneBalanceAccount**'
  name: surcharge
  type: string
- description: 'Specifies the logic to apply when booking tips (gratuity). Possible values: **addToLiableAccount**, **addToOneBalanceAccount**.'
  name: tip
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-update-split-configuration-logic-request-schema.json
slug: management-update-split-configuration-logic-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-split-configuration-logic-request-schema.json\",\n  \"title\": \"UpdateSplitConfigurationLogicRequest\",\n  \"description\": \"UpdateSplitConfigurationLogicRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acquiringFees\": {\n      \"description\": \"Specifies the logic to apply when booking the transaction fees. Should be combined with adyenFees.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"additionalCommission\": {\n      \"description\": \"Contains the logic used to calculate your user's commission, booked directly to their balance account.\",\n      \"$ref\": \"#/components/schemas/AdditionalCommission\"\
  \n    },\n    \"adyenCommission\": {\n      \"description\": \"Specifies the logic to apply when booking the transaction fees. Should be combined with schemeFee, interchange & adyenMarkup.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"adyenFees\": {\n      \"description\": \"Specifies the logic to apply when booking the transaction fees. Should be combined with acquiringFees.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"adyenMarkup\": {\n      \"description\": \"Specifies the logic to apply when booking the transaction fees. Should be combined with schemeFee, adyenCommission & interchange.\\n\\nPossible values:\
  \ **deductFromLiableAccount**, **deductFromOneBalanceAccount**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"chargeback\": {\n      \"description\": \"Specifies the logic to apply when booking the chargeback amount.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**, **deductAccordingToSplitRatio**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\",\n        \"deductAccordingToSplitRatio\"\n      ],\n      \"type\": \"string\"\n    },\n    \"chargebackCostAllocation\": {\n      \"description\": \"Specifies the logic to apply when allocating the chargeback costs.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"commission\"\
  : {\n      \"description\": \"Contains the logic used to the calculate your platform's commission, booked to your liable balance account.\",\n      \"$ref\": \"#/components/schemas/Commission\"\n    },\n    \"interchange\": {\n      \"description\": \"Specifies the logic to apply when booking the transaction fees. Should be combined with schemeFee, adyenCommission & adyenMarkup.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"paymentFee\": {\n      \"description\": \"Specifies the logic to apply when booking the transaction fees. Cannot be combined with other fees.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"\
  remainder\": {\n      \"description\": \"Specifies the logic to apply when booking the amount left over after currency conversion.\\n\\nPossible values: **addToLiableAccount**, **addToOneBalanceAccount**.\",\n      \"enum\": [\n        \"addToLiableAccount\",\n        \"addToOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"schemeFee\": {\n      \"description\": \"Specifies the logic to apply when booking the transaction fees. Should be combined with interchange, adyenCommission & adyenMarkup.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**.\",\n      \"enum\": [\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"splitLogicId\": {\n      \"description\": \"Unique identifier of the split logic that is applied when the split configuration conditions are met.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"surcharge\": {\n    \
  \  \"description\": \"Specifies the logic to apply when booking the surcharge amount.\\n\\nPossible values: **addToLiableAccount**, **addToOneBalanceAccount**\",\n      \"enum\": [\n        \"addToLiableAccount\",\n        \"addToOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"tip\": {\n      \"description\": \"Specifies the logic to apply when booking tips (gratuity).\\n\\nPossible values: **addToLiableAccount**, **addToOneBalanceAccount**.\",\n      \"enum\": [\n        \"addToLiableAccount\",\n        \"addToOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"commission\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-split-configuration-logic-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateSplitConfigurationLogicRequest
---
