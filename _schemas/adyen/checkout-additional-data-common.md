---
description: AdditionalDataCommon schema from Adyen API
layout: schema
name: AdditionalDataCommon
properties_list:
- description: 'Triggers test scenarios that allow to replicate certain communication errors. Allowed values: * **NO_CONNECTION_AVAILABLE** – There wasn''t a connection available to service the outgoing communication.'
  name: RequestedTestErrorResponseCode
  type: string
- description: 'Set to true to authorise a part of the requested amount in case the cardholder does not have enough funds on their account. If a payment was partially authorised, the response includes resultCode: Par'
  name: allowPartialAuth
  type: string
- description: Flags a card payment request for either pre-authorisation or final authorisation. For more information, refer to [Authorisation types](https://docs.adyen.com/online-payments/adjust-authorisation#autho
  name: authorisationType
  type: string
- description: Allows you to determine or override the acquirer account that should be used for the transaction. If you need to process a payment with an acquirer different from a default one, you can set up a corre
  name: customRoutingFlag
  type: string
- description: In case of [asynchronous authorisation adjustment](https://docs.adyen.com/online-payments/adjust-authorisation#adjust-authorisation), this field denotes why the additional payment is made. Possible va
  name: industryUsage
  type: string
- description: Set to **true** to require [manual capture](https://docs.adyen.com/online-payments/capture) for the transaction.
  name: manualCapture
  type: string
- description: Allows you to link the transaction to the original or previous one in a subscription/card-on-file chain. This field is required for token-based transactions where Adyen does not tokenize the card. Tra
  name: networkTxReference
  type: string
- description: Boolean indicator that can be optionally used for performing debit transactions on combo cards (for example, combo cards in Brazil). This is not mandatory but we recommend that you set this to true if
  name: overwriteBrand
  type: string
- description: 'This field is required if the transaction is performed by a registered payment facilitator. This field must contain the city of the actual merchant''s address. * Format: alpha-numeric. * Maximum length'
  name: subMerchantCity
  type: string
- description: 'This field is required if the transaction is performed by a registered payment facilitator. This field must contain the three-letter country code of the actual merchant''s address. * Format: alpha-nume'
  name: subMerchantCountry
  type: string
- description: This field contains an identifier of the actual merchant when a transaction is submitted via a payment facilitator. The payment facilitator must send in this unique ID. A unique identifier per submerc
  name: subMerchantID
  type: string
- description: 'This field is required if the transaction is performed by a registered payment facilitator. This field must contain the name of the actual merchant. * Format: alpha-numeric. * Maximum length: 22 chara'
  name: subMerchantName
  type: string
- description: 'This field is required if the transaction is performed by a registered payment facilitator. This field must contain the postal code of the actual merchant''s address. * Format: alpha-numeric. * Maximum'
  name: subMerchantPostalCode
  type: string
- description: This field is required if the transaction is performed by a registered payment facilitator, and if applicable to the country. This field must contain the state code of the actual merchant's address. *
  name: subMerchantState
  type: string
- description: 'This field is required if the transaction is performed by a registered payment facilitator. This field must contain the street of the actual merchant''s address. * Format: alpha-numeric. * Maximum leng'
  name: subMerchantStreet
  type: string
- description: 'This field is required if the transaction is performed by a registered payment facilitator. This field must contain the tax ID of the actual merchant. * Format: alpha-numeric. * Fixed length: 11 or 14'
  name: subMerchantTaxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-additional-data-common-schema.json
slug: checkout-additional-data-common
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-common-schema.json\",\n  \"title\": \"AdditionalDataCommon\",\n  \"description\": \"AdditionalDataCommon schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestedTestErrorResponseCode\": {\n      \"description\": \"Triggers test scenarios that allow to replicate certain communication errors.\\n\\nAllowed values:\\n* **NO_CONNECTION_AVAILABLE** \\u2013 There wasn't a connection available to service the outgoing communication.\\nThis is a transient, retriable error since no messaging could be initiated to an issuing system (or third-party acquiring system). Therefore, the header Transient-Error: true is returned in the response. A subsequent request using the same idempotency key will be processed as if it was the first request.\\n* **IOEXCEPTION_RECEIVED** \\\
  u2013 Something went wrong during transmission of the message or receiving the response.\\nThis is a classified as non-transient because the message could have been received by the issuing party and been acted upon. No transient error header is returned. If using idempotency, the (error) response is stored as the final result for the idempotency key. Subsequent messages with the same idempotency key not be processed beyond returning the stored response.\",\n      \"type\": \"string\"\n    },\n    \"allowPartialAuth\": {\n      \"description\": \"Set to true to authorise a part of the requested amount in case the cardholder does not have enough funds on their account. \\nIf a payment was partially authorised, the response includes resultCode: PartiallyAuthorised and the authorised amount in additionalData.authorisedAmountValue.\\nTo enable this functionality, contact our Support Team.\",\n      \"type\": \"string\"\n    },\n    \"authorisationType\": {\n      \"description\": \"Flags a\
  \ card payment request for either pre-authorisation or final authorisation. For more information, refer to [Authorisation types](https://docs.adyen.com/online-payments/adjust-authorisation#authorisation-types).\\n\\nAllowed values:\\n* **PreAuth** \\u2013 flags the payment request to be handled as a pre-authorisation.\\n* **FinalAuth** \\u2013 flags the payment request to be handled as a final authorisation.\",\n      \"type\": \"string\"\n    },\n    \"customRoutingFlag\": {\n      \"description\": \"Allows you to determine or override the acquirer account that should be used for the transaction.\\n\\nIf you need to process a payment with an acquirer different from a default one, you can set up a corresponding configuration on the Adyen payments platform. Then you can pass a custom routing flag in a payment request's additional data to target a specific acquirer.\\n\\nTo enable this functionality, contact [Support](https://www.adyen.help/hc/en-us/requests/new).\",\n      \"type\": \"\
  string\"\n    },\n    \"industryUsage\": {\n      \"description\": \"In case of [asynchronous authorisation adjustment](https://docs.adyen.com/online-payments/adjust-authorisation#adjust-authorisation), this field denotes why the additional payment is made.\\n\\nPossible values:\\n\\n * **NoShow**: An incremental charge is carried out because of a no-show for a guaranteed reservation.\\n\\n * **DelayedCharge**: An incremental charge is carried out to process an additional payment after the original services have been rendered and the respective payment has been processed.\",\n      \"enum\": [\n        \"NoShow\",\n        \"DelayedCharge\"\n      ],\n      \"type\": \"string\"\n    },\n    \"manualCapture\": {\n      \"description\": \"Set to **true** to require [manual capture](https://docs.adyen.com/online-payments/capture) for the transaction.\",\n      \"type\": \"string\"\n    },\n    \"networkTxReference\": {\n      \"description\": \"Allows you to link the transaction to the original\
  \ or previous one in a subscription/card-on-file chain. This field is required for token-based transactions where Adyen does not tokenize the card.\\n\\nTransaction identifier from card schemes, for example, Mastercard Trace ID or the Visa Transaction ID.\\n\\nSubmit the original transaction ID of the contract in your payment request if you are not tokenizing card details with Adyen and are making a merchant-initiated transaction (MIT) for subsequent charges.\\n\\nMake sure you are sending `shopperInteraction` **ContAuth** and `recurringProcessingModel` **Subscription** or **UnscheduledCardOnFile** to ensure that the transaction is classified as MIT.\",\n      \"type\": \"string\"\n    },\n    \"overwriteBrand\": {\n      \"description\": \"Boolean indicator that can be optionally used for performing debit transactions on combo cards (for example, combo cards in Brazil). This is not mandatory but we recommend that you set this to true if you want to use the `selectedBrand` value to specify\
  \ how to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantCity\": {\n      \"description\": \"This field is required if the transaction is performed by a registered payment facilitator. This field must contain the city of the actual merchant's address.\\n* Format: alpha-numeric.\\n* Maximum length: 13 characters.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantCountry\": {\n      \"description\": \"This field is required if the transaction is performed by a registered payment facilitator. This field must contain the three-letter country code of the actual merchant's address.\\n* Format: alpha-numeric.\\n* Fixed length: 3 characters.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantID\": {\n      \"description\": \"This field contains an identifier of the actual merchant when a transaction is submitted via a payment facilitator. The payment facilitator must send in this unique ID.\\n\\nA unique identifier per submerchant that is required\
  \ if the transaction is performed by a registered payment facilitator.\\n* Format: alpha-numeric.\\n* Fixed length: 15 characters.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantName\": {\n      \"description\": \"This field is required if the transaction is performed by a registered payment facilitator. This field must contain the name of the actual merchant.\\n* Format: alpha-numeric.\\n* Maximum length: 22 characters.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantPostalCode\": {\n      \"description\": \"This field is required if the transaction is performed by a registered payment facilitator. This field must contain the postal code of the actual merchant's address.\\n* Format: alpha-numeric.\\n* Maximum length: 10 characters.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantState\": {\n      \"description\": \"This field is required if the transaction is performed by a registered payment facilitator, and if applicable to the country. This field must contain\
  \ the state code of the actual merchant's address.\\n* Format: alpha-numeric.\\n* Maximum length: 3 characters.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantStreet\": {\n      \"description\": \"This field is required if the transaction is performed by a registered payment facilitator. This field must contain the street of the actual merchant's address.\\n* Format: alpha-numeric.\\n* Maximum length: 60 characters.\",\n      \"type\": \"string\"\n    },\n    \"subMerchantTaxId\": {\n      \"description\": \"This field is required if the transaction is performed by a registered payment facilitator. This field must contain the tax ID of the actual merchant.\\n* Format: alpha-numeric.\\n* Fixed length: 11 or 14 characters.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-common-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataCommon
---
