---
description: ThreeDS2RequestFields schema from Adyen API
layout: schema
name: ThreeDS2RequestFields
properties_list:
- description: Additional information about the Cardholder’s account provided by the 3DS Requestor.
  name: acctInfo
  type: object
- description: 'Indicates the type of account. For example, for a multi-account card product. Length: 2 characters. Allowed values: * **01** — Not applicable * **02** — Credit * **03** — Debit'
  name: acctType
  type: string
- description: Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only). The acquiring BIN enrolled for 3D Secure 2. This string should mat
  name: acquirerBIN
  type: string
- description: 'Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only). The merchantId that is enrolled for 3D Secure 2 by the merchant''s '
  name: acquirerMerchantID
  type: string
- description: 'Indicates whether the Cardholder Shipping Address and Cardholder Billing Address are the same. Allowed values: * **Y** — Shipping Address matches Billing Address. * **N** — Shipping Address does not m'
  name: addrMatch
  type: string
- description: If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation.
  name: authenticationOnly
  type: boolean
- description: 'Possibility to specify a preference for receiving a challenge from the issuer. Allowed values: * `noPreference` * `requestNoChallenge` * `requestChallenge` * `requestChallengeAsMandate`'
  name: challengeIndicator
  type: string
- description: Display options for the 3D Secure 2 SDK. Optional and only for `deviceChannel` **app**.
  name: deviceRenderOptions
  type: object
- description: The home phone number provided by the Cardholder.
  name: homePhone
  type: object
- description: Required for merchants that have been enrolled for 3D Secure 2 by another party than Adyen, mostly [authentication-only integrations](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/a
  name: mcc
  type: string
- description: 'Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only). The merchant name that the issuer presents to the shopper if they '
  name: merchantName
  type: string
- description: The `messageVersion` value indicating the 3D Secure 2 protocol version.
  name: messageVersion
  type: string
- description: The mobile phone number provided by the Cardholder.
  name: mobilePhone
  type: object
- description: URL to where the issuer should send the `CRes`. Required if you are not using components for `channel` **Web** or if you are using classic integration `deviceChannel` **browser**.
  name: notificationURL
  type: string
- description: Value **true** indicates that the transaction was de-tokenised prior to being received by the ACS.
  name: payTokenInd
  type: boolean
- description: Indicates the type of payment for which an authentication is requested (message extension)
  name: paymentAuthenticationUseCase
  type: string
- description: 'The platform of the shopper. Allowed values: * `iOS` * `android` * `browser`'
  name: platform
  type: string
- description: 'Indicates the maximum number of authorisations permitted for instalment payments. Length: 1–3 characters.'
  name: purchaseInstalData
  type: string
- description: 'Date after which no further authorisations shall be performed. Format: YYYYMMDD'
  name: recurringExpiry
  type: string
- description: 'Indicates the minimum number of days between authorisations. Maximum length: 4 characters.'
  name: recurringFrequency
  type: string
- description: The `sdkAppID` value as received from the 3D Secure 2 SDK.
  name: sdkAppID
  type: string
- description: The `sdkEphemPubKey` value as received from the 3D Secure 2 SDK.
  name: sdkEphemPubKey
  type: object
- description: The maximum amount of time in minutes for the 3D Secure 2 authentication process. Optional and only for `deviceChannel` set to **app**. Defaults to **60** minutes.
  name: sdkMaxTimeout
  type: integer
- description: The `sdkReferenceNumber` value as received from the 3D Secure 2 SDK.
  name: sdkReferenceNumber
  type: string
- description: The `sdkTransID` value as received from the 3D Secure 2 SDK.
  name: sdkTransID
  type: string
- description: Completion indicator for the device fingerprinting.
  name: threeDSCompInd
  type: string
- description: Indicates the type of Authentication request.
  name: threeDSRequestorAuthenticationInd
  type: string
- description: Information about how the 3DS Requestor authenticated the cardholder before or during the transaction
  name: threeDSRequestorAuthenticationInfo
  type: object
- description: 'Indicates whether a challenge is requested for this transaction. Possible values: * **01** — No preference * **02** — No challenge requested * **03** — Challenge requested (3DS Requestor preference) *'
  name: threeDSRequestorChallengeInd
  type: string
- description: Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only) for Visa. Unique 3D Secure requestor identifier assigned by the Dir
  name: threeDSRequestorID
  type: string
- description: Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only) for Visa. Unique 3D Secure requestor name assigned by the Directory
  name: threeDSRequestorName
  type: string
- description: Information about how the 3DS Requestor authenticated the cardholder as part of a previous 3DS transaction.
  name: threeDSRequestorPriorAuthenticationInfo
  type: object
- description: URL of the (customer service) website that will be shown to the shopper in case of technical errors during the 3D Secure 2 process.
  name: threeDSRequestorURL
  type: string
- description: 'Identifies the type of transaction being authenticated. Length: 2 characters. Allowed values: * **01** — Goods/Service Purchase * **03** — Check Acceptance * **10** — Account Funding * **11** — Quasi-'
  name: transType
  type: string
- description: Identify the type of the transaction being authenticated.
  name: transactionType
  type: string
- description: The `whiteListStatus` value returned from a previous 3D Secure 2 transaction, only applicable for 3D Secure 2 protocol version 2.2.0.
  name: whiteListStatus
  type: string
- description: The work phone number provided by the Cardholder.
  name: workPhone
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-three-ds2-request-fields-schema.json
slug: checkout-three-ds2-request-fields
source_filename: checkout-three-ds2-request-fields-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds2-request-fields-schema.json\",\n  \"title\": \"ThreeDS2RequestFields\",\n  \"description\": \"ThreeDS2RequestFields schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acctInfo\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Additional information about the Cardholder\\u2019s account provided by the 3DS Requestor.\",\n      \"$ref\": \"#/components/schemas/AcctInfo\"\n    },\n    \"acctType\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates the type of account. For example, for a multi-account card product. Length: 2 characters. Allowed values:\\n* **01** \\u2014 Not applicable\\n* **02** \\u2014 Credit\\n* **03** \\u2014 Debit\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\"\n      ],\n      \"maxLength\"\
  : 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"acquirerBIN\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only). The acquiring BIN enrolled for 3D Secure 2. This string should match the value that you will use in the authorisation. Use 123456 on the Test platform.\",\n      \"type\": \"string\"\n    },\n    \"acquirerMerchantID\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only). The merchantId that is enrolled for 3D Secure 2 by the merchant's acquirer. This string should match the value that you will use in the authorisation. Use 123456 on the Test platform.\",\n      \"type\": \"string\"\n    },\n    \"addrMatch\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\"\
  : \"Indicates whether the Cardholder Shipping Address and Cardholder Billing Address are the same. Allowed values:\\n* **Y** \\u2014 Shipping Address matches Billing Address.\\n* **N** \\u2014 Shipping Address does not match Billing Address.\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ],\n      \"maxLength\": 1,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"authenticationOnly\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"50\",\n      \"x-deprecatedMessage\": \"Use `threeDSAuthenticationOnly` instead.\",\n      \"default\": false,\n      \"description\": \"If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation.\",\n      \"type\": \"boolean\"\n    },\n    \"challengeIndicator\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"68\",\n      \"x-deprecatedMessage\": \"Use `threeDSRequestorChallengeInd`\
  \ instead.\",\n      \"description\": \"Possibility to specify a preference for receiving a challenge from the issuer.\\nAllowed values:\\n* `noPreference`\\n* `requestNoChallenge`\\n* `requestChallenge`\\n* `requestChallengeAsMandate`\\n\",\n      \"enum\": [\n        \"noPreference\",\n        \"requestNoChallenge\",\n        \"requestChallenge\",\n        \"requestChallengeAsMandate\"\n      ],\n      \"type\": \"string\"\n    },\n    \"deviceRenderOptions\": {\n      \"description\": \"Display options for the 3D Secure 2 SDK.\\nOptional and only for `deviceChannel` **app**.\",\n      \"$ref\": \"#/components/schemas/DeviceRenderOptions\"\n    },\n    \"homePhone\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The home phone number provided by the Cardholder.\",\n      \"$ref\": \"#/components/schemas/Phone\"\n    },\n    \"mcc\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"Required for merchants that have been enrolled for 3D Secure 2 by another\
  \ party than Adyen, mostly [authentication-only integrations](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only). The `mcc` is a four-digit code with which the previously given `acquirerMerchantID` is registered at the scheme.\",\n      \"type\": \"string\"\n    },\n    \"merchantName\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only). The merchant name that the issuer presents to the shopper if they get a challenge. We recommend to use the same value that you will use in the authorization. Maximum length is 40 characters.\\n> Optional for a [full 3D Secure 2 integration](https://docs.adyen.com/online-payments/3d-secure/native-3ds2/api-integration). Use this field if you are enrolled for 3D Secure 2 with us and want to override the merchant name already configured on your account.\",\n      \"type\": \"\
  string\"\n    },\n    \"messageVersion\": {\n      \"description\": \"The `messageVersion` value indicating the 3D Secure 2 protocol version.\",\n      \"type\": \"string\"\n    },\n    \"mobilePhone\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The mobile phone number provided by the Cardholder.\",\n      \"$ref\": \"#/components/schemas/Phone\"\n    },\n    \"notificationURL\": {\n      \"description\": \"URL to where the issuer should send the `CRes`. Required if you are not using components for `channel` **Web** or if you are using classic integration `deviceChannel` **browser**.\",\n      \"type\": \"string\"\n    },\n    \"payTokenInd\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Value **true** indicates that the transaction was de-tokenised prior to being received by the ACS.\",\n      \"type\": \"boolean\"\n    },\n    \"paymentAuthenticationUseCase\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates the type\
  \ of payment for which an authentication is requested (message extension)\",\n      \"type\": \"string\"\n    },\n    \"platform\": {\n      \"description\": \"The platform of the shopper.\\nAllowed values:\\n* `iOS`\\n* `android`\\n* `browser`\",\n      \"enum\": [\n        \"iOS\",\n        \"android\",\n        \"browser\"\n      ],\n      \"type\": \"string\"\n    },\n    \"purchaseInstalData\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates the maximum number of authorisations permitted for instalment payments. Length: 1\\u20133 characters.\",\n      \"maxLength\": 3,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"recurringExpiry\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Date after which no further authorisations shall be performed. Format: YYYYMMDD\",\n      \"type\": \"string\"\n    },\n    \"recurringFrequency\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates the minimum number\
  \ of days between authorisations. Maximum length: 4 characters.\",\n      \"maxLength\": 4,\n      \"type\": \"string\"\n    },\n    \"sdkAppID\": {\n      \"description\": \"The `sdkAppID` value as received from the 3D Secure 2 SDK.\",\n      \"type\": \"string\"\n    },\n    \"sdkEphemPubKey\": {\n      \"description\": \"The `sdkEphemPubKey` value as received from the 3D Secure 2 SDK.\",\n      \"$ref\": \"#/components/schemas/SDKEphemPubKey\"\n    },\n    \"sdkMaxTimeout\": {\n      \"default\": 60,\n      \"description\": \"The maximum amount of time in minutes for the 3D Secure 2 authentication process.\\nOptional and only for `deviceChannel` set to **app**. Defaults to **60** minutes.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"sdkReferenceNumber\": {\n      \"description\": \"The `sdkReferenceNumber` value as received from the 3D Secure 2 SDK.\",\n      \"type\": \"string\"\n    },\n    \"sdkTransID\": {\n      \"description\": \"The `sdkTransID`\
  \ value as received from the 3D Secure 2 SDK.\",\n      \"type\": \"string\"\n    },\n    \"threeDSCompInd\": {\n      \"description\": \"Completion indicator for the device fingerprinting.\",\n      \"type\": \"string\"\n    },\n    \"threeDSRequestorAuthenticationInd\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates the type of Authentication request.\",\n      \"type\": \"string\"\n    },\n    \"threeDSRequestorAuthenticationInfo\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Information about how the 3DS Requestor authenticated the cardholder before or during the transaction\",\n      \"$ref\": \"#/components/schemas/ThreeDSRequestorAuthenticationInfo\"\n    },\n    \"threeDSRequestorChallengeInd\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates whether a challenge is requested for this transaction. Possible values:\\n* **01** \\u2014 No preference\\n* **02** \\u2014 No challenge requested\\n* **03** \\u2014\
  \ Challenge requested (3DS Requestor preference)\\n* **04** \\u2014 Challenge requested (Mandate)\\n* **05** \\u2014 No challenge (transactional risk analysis is already performed)\\n* **06** \\u2014 Data Only\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"06\"\n      ],\n      \"type\": \"string\"\n    },\n    \"threeDSRequestorID\": {\n      \"description\": \"Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only) for Visa. Unique 3D Secure requestor identifier assigned by the Directory Server when you enrol for 3D Secure 2.\",\n      \"type\": \"string\"\n    },\n    \"threeDSRequestorName\": {\n      \"description\": \"Required for [authentication-only integration](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only) for Visa. Unique 3D Secure requestor name assigned by the Directory Server when you enrol\
  \ for 3D Secure 2.\",\n      \"type\": \"string\"\n    },\n    \"threeDSRequestorPriorAuthenticationInfo\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Information about how the 3DS Requestor authenticated the cardholder as part of a previous 3DS transaction.\",\n      \"$ref\": \"#/components/schemas/ThreeDSRequestorPriorAuthenticationInfo\"\n    },\n    \"threeDSRequestorURL\": {\n      \"description\": \"URL of the (customer service) website that will be shown to the shopper in case of technical errors during the 3D Secure 2 process.\",\n      \"type\": \"string\"\n    },\n    \"transType\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Identifies the type of transaction being authenticated. Length: 2 characters. Allowed values:\\n* **01** \\u2014 Goods/Service Purchase\\n* **03** \\u2014 Check Acceptance\\n* **10** \\u2014 Account Funding\\n* **11** \\u2014 Quasi-Cash Transaction\\n* **28** \\u2014 Prepaid Activation and Load\",\n      \"enum\"\
  : [\n        \"01\",\n        \"03\",\n        \"10\",\n        \"11\",\n        \"28\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"transactionType\": {\n      \"x-addedInVersion\": \"50\",\n      \"description\": \"Identify the type of the transaction being authenticated.\",\n      \"enum\": [\n        \"goodsOrServicePurchase\",\n        \"checkAcceptance\",\n        \"accountFunding\",\n        \"quasiCashTransaction\",\n        \"prepaidActivationAndLoad\"\n      ],\n      \"type\": \"string\"\n    },\n    \"whiteListStatus\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"The `whiteListStatus` value returned from a previous 3D Secure 2 transaction, only applicable for 3D Secure 2 protocol version 2.2.0.\",\n      \"type\": \"string\"\n    },\n    \"workPhone\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The work phone number provided by the Cardholder.\",\n      \"$ref\": \"#/components/schemas/Phone\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds2-request-fields-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDS2RequestFields
---
