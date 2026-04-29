---
description: ''
layout: schema
name: TransactionInsightsData
properties_list:
- description: The purchase date in format YYYYMMDDHHMMSS
  name: purchaseDate
  type: string
- description: The amount of the transaction in the currency's basic unit. If the purchase amount is USD 123.45, element will contain the value 12345. Max value is MAX_LONG (9223372036854775807)
  name: purchaseAmount
  type: string
- description: The Purchase currency Exponent. If the purchase amount is USD 123.45, then the exponent will contain 2.
  name: purchaseCurrencyExponent
  type: string
- description: 'The currency of the transaction amount, as an ISO-4217 currency code. See: [ISO-4217](https://www.nationsonline.org/oneworld/currencies.htm)'
  name: purchaseCurrency
  type: string
- description: The name of the business.
  name: merchantName
  type: string
- description: 'The ISO-3166 numeric country code of the merchant associated with the transaction. See: [ISO-3166](https://www.nationsonline.org/oneworld/country_code_list.htm).'
  name: merchantCountryCode
  type: string
- description: The Merchant Category Code associated with the transaction.
  name: mcc
  type: string
- description: 'IPv4 address is represented in the dotted decimal format of 4 sets of decimal numbers separated by dots. The decimal number in each and every set is in the range 0 to 255. IPv6 address is represented '
  name: ipAddress
  type: string
- description: The user-agent string of the consumer device attempting to authorize with your product or service. The user-agent must represent the HTTP client of the service consumer with details on the software or
  name: userAgent
  type: string
- description: The canvas signature of the browser installed on the consumer device.
  name: canvas
  type: string
- description: The webGL signature of the browser installed on the consumer device.
  name: webGl
  type: string
- description: Time-zone of the consumer device. The timezone must be a number of the time-zone offset, in minutes, from the date based on current host system settings to UTC.
  name: timeZone
  type: string
- description: The screen resolution of the consumer device attempting to authorize with your product or service.
  name: screenResolution
  type: string
- description: Flag to local storage is enabled on the consumer device.
  name: localStorage
  type: boolean
- description: The language of the consumer device. The language must be a string representing the language version as defined in BCP-47.
  name: language
  type: string
- description: The device screen color depth value.
  name: colorDepth
  type: integer
- description: Manufacturer of the product/hardware.
  name: buildManufacturer
  type: string
- description: This optional field contains the placement identifier within the application.
  name: placement
  type: string
- description: Build is used to determine information about the current build, extracted from system properties.
  name: androidBuildVersion
  type: string
- description: The user-visible SDK version of the framework; its possible values are defined in Build.VERSION_CODES.
  name: androidSdkInt
  type: string
- description: String that uniquely identifies this build.
  name: buildFingerprint
  type: string
- description: Consumer-visible brand with which the product/hardware will be associated, if any.
  name: buildBrand
  type: string
- description: List of the supported features on the consumer device.
  name: supportedFeatures
  type: array
- description: 'Mobile device manufacturer and modelAndroid: Build.MANUFACTURER + " " + Build.MODEL returns the mobile device manufacturer and model, For example,"samsung SM-G960U1", iOS: utsname.machine returns the '
  name: model
  type: string
- description: 'The unique package name/bundle identifier of the client''s application. Android: obtained from the applicationContext.getPackageName() method. iOS: obtained from the [NSBundle mainBundle] bundleIdentif'
  name: sdkUserAgent
  type: string
- description: Major operating system version.
  name: majorOsVersion
  type: integer
- description: Minor operating system version.
  name: minorOsVersion
  type: integer
- description: ISO country code equivalent for the SIM provider's country code.
  name: simCountryIso
  type: string
- description: MCC+MNC (mobile country code + mobile network code) of the SIM provider.
  name: simOperator
  type: string
- description: Device primary storage size.
  name: primaryStorage
  type: integer
- description: Device System memory size.
  name: systemMemory
  type: integer
- description: Name of the overall product.
  name: buildProduct
  type: string
- description: Alphanumeric string that uniquely identifies a device to the app vendor.
  name: vendorAppId
  type: string
- description: Optional unique device identifier that merchant can store on consumer device. E.g with cookie in web flow.
  name: storedDeviceId
  type: string
- description: Google's unique device identifier. A 64-bit number (as a hex string) that is randomly generated when the end user first sets up the device.
  name: androidId
  type: string
- description: The hashed account identifier used during the authorization attempt.
  name: hashedAccountId
  type: string
- description: The End Customer Reference identifier is used during the reseller transaction request.
  name: endCustomerRefId
  type: string
- description: Flag to indicate cookies are enabled on the consumer device.
  name: cookiesEnabled
  type: boolean
- description: A list of browser plugins.
  name: plugins
  type: array
- description: The merchant ID that the transaction was processed under, as assigned by the acquirer.
  name: acquirerMerchantId
  type: string
- description: The BIN (Bank Identification Number) of the acquirer.
  name: acquirerBin
  type: string
- description: The full name of the person.
  name: cardHolderName
  type: string
- description: The full name of the person.
  name: secondaryName
  type: string
- description: The primary contact detail - Email id
  name: primaryEmail
  type: string
- description: Secondary email to contact if primary details are not reachable
  name: secondaryEmail
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-transaction-insights-data-schema.json
slug: mastercard-identity-insights-for-transactions-transaction-insights-data
source_filename: mastercard-identity-insights-for-transactions-transaction-insights-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionInsightsData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"purchaseDate\": {\n      \"type\": \"string\",\n      \"description\": \"The purchase date in format YYYYMMDDHHMMSS\"\n    },\n    \"purchaseAmount\": {\n      \"type\": \"string\",\n      \"description\": \"The amount of the transaction in the currency's basic unit. If the purchase amount is USD 123.45, element will contain the value 12345. Max value is MAX_LONG (9223372036854775807)\"\n    },\n    \"purchaseCurrencyExponent\": {\n      \"type\": \"string\",\n      \"description\": \"The Purchase currency Exponent. If the purchase amount is USD 123.45, then the exponent will contain 2.\"\n    },\n    \"purchaseCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency of the transaction amount, as an ISO-4217 currency code. See: [ISO-4217](https://www.nationsonline.org/oneworld/currencies.htm)\"\
  \n    },\n    \"merchantName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the business.\"\n    },\n    \"merchantCountryCode\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO-3166 numeric country code of the merchant associated with the transaction. See: [ISO-3166](https://www.nationsonline.org/oneworld/country_code_list.htm).\"\n    },\n    \"mcc\": {\n      \"type\": \"string\",\n      \"description\": \"The Merchant Category Code associated with the transaction.\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"description\": \"IPv4 address is represented in the dotted decimal format of 4 sets\\nof decimal numbers separated by dots. The decimal number in each and\\nevery set is in the range 0 to 255. IPv6 address is represented as\\neight groups of four hexadecimal digits, each group representing 16\\nbits (two octets. The groups are separated by colons (:).\\n- Optional to generate individual insights\\n- Required to\
  \ generate device insights\"\n    },\n    \"userAgent\": {\n      \"type\": \"string\",\n      \"description\": \"The user-agent string of the consumer device attempting to authorize\\nwith your product or service. The user-agent must represent the HTTP\\nclient of the service consumer with details on the software\\noriginating the request.\\n- Optional to generate individual insights\\n- Required to generate device insights\"\n    },\n    \"canvas\": {\n      \"type\": \"string\",\n      \"description\": \"The canvas signature of the browser installed on the consumer device.\"\n    },\n    \"webGl\": {\n      \"type\": \"string\",\n      \"description\": \"The webGL signature of the browser installed on the consumer device.\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Time-zone of the consumer device. The timezone must be a number of the time-zone offset, in minutes, from the date based on current host system settings to UTC.\"\n    },\n    \"\
  screenResolution\": {\n      \"type\": \"string\",\n      \"description\": \"The screen resolution of the consumer device attempting to authorize with your product or service.\"\n    },\n    \"localStorage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag to local storage is enabled on the consumer device.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the consumer device. The language must be a string representing the language version as defined in BCP-47.\"\n    },\n    \"colorDepth\": {\n      \"type\": \"integer\",\n      \"description\": \"The device screen color depth value.\"\n    },\n    \"buildManufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer of the product/hardware.\"\n    },\n    \"placement\": {\n      \"type\": \"string\",\n      \"description\": \"This optional field contains the placement identifier within the application.\"\n    },\n    \"androidBuildVersion\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Build is used to determine information about the current build, extracted from system properties.\"\n    },\n    \"androidSdkInt\": {\n      \"type\": \"string\",\n      \"description\": \"The user-visible SDK version of the framework; its possible values are defined in Build.VERSION_CODES.\"\n    },\n    \"buildFingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"String that uniquely identifies this build.\"\n    },\n    \"buildBrand\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer-visible brand with which the product/hardware will be associated, if any.\"\n    },\n    \"supportedFeatures\": {\n      \"type\": \"array\",\n      \"description\": \"List of the supported features on the consumer device.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile device manufacturer and modelAndroid: Build.MANUFACTURER + \\\" \\\" + Build.MODEL returns the mobile device\
  \ manufacturer and model, For example,\\\"samsung SM-G960U1\\\",\\n\\niOS: utsname.machine returns the device model, For example, \\\"iPhone10.4\\\". Note: Apple as a manufacturer is not included because it is the same for all iOS devices.\"\n    },\n    \"sdkUserAgent\": {\n      \"type\": \"string\",\n      \"description\": \"The unique package name/bundle identifier of the client's application.\\n\\nAndroid: obtained from the applicationContext.getPackageName() method.\\n\\niOS: obtained from the [NSBundle mainBundle] bundleIdentifier property.\"\n    },\n    \"majorOsVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"Major operating system version.\"\n    },\n    \"minorOsVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"Minor operating system version.\"\n    },\n    \"simCountryIso\": {\n      \"type\": \"string\",\n      \"description\": \"ISO country code equivalent for the SIM provider's country code.\"\n    },\n    \"simOperator\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"MCC+MNC (mobile country code + mobile network code) of the SIM provider.\"\n    },\n    \"primaryStorage\": {\n      \"type\": \"integer\",\n      \"description\": \"Device primary storage size.\"\n    },\n    \"systemMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"Device System memory size.\"\n    },\n    \"buildProduct\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the overall product.\"\n    },\n    \"vendorAppId\": {\n      \"type\": \"string\",\n      \"description\": \"Alphanumeric string that uniquely identifies a device to the app vendor.\"\n    },\n    \"storedDeviceId\": {\n      \"type\": \"string\",\n      \"description\": \"Optional unique device identifier that merchant can store on consumer device. E.g with cookie in web flow.\"\n    },\n    \"androidId\": {\n      \"type\": \"string\",\n      \"description\": \"Google's unique device identifier. A 64-bit number (as a hex string)\
  \ that is randomly generated when the end user first sets up the device.\"\n    },\n    \"hashedAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The hashed account identifier used during the authorization attempt.\"\n    },\n    \"endCustomerRefId\": {\n      \"type\": \"string\",\n      \"description\": \"The End Customer Reference identifier is used during the reseller transaction request.\"\n    },\n    \"cookiesEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag to indicate cookies are enabled on the consumer device.\"\n    },\n    \"plugins\": {\n      \"type\": \"array\",\n      \"description\": \"A list of browser plugins.\"\n    },\n    \"acquirerMerchantId\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant ID that the transaction was processed under, as assigned by the acquirer.\"\n    },\n    \"acquirerBin\": {\n      \"type\": \"string\",\n      \"description\": \"The BIN (Bank Identification Number) of the acquirer.\"\
  \n    },\n    \"cardHolderName\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the person.\"\n    },\n    \"secondaryName\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the person.\"\n    },\n    \"primaryEmail\": {\n      \"type\": \"string\",\n      \"description\": \"The primary contact detail - Email id\"\n    },\n    \"secondaryEmail\": {\n      \"type\": \"string\",\n      \"description\": \"Secondary email to contact if primary details are not reachable\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-transaction-insights-data-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: TransactionInsightsData
---
