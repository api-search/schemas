---
description: AccountHolderDetails schema from Adyen API
layout: schema
name: AccountHolderDetails
properties_list:
- description: The address of the account holder.
  name: address
  type: object
- description: Array of bank accounts associated with the account holder. For details about the required `bankAccountDetail` fields, see [Required information](https://docs.adyen.com/marketplaces-and-platforms/class
  name: bankAccountDetails
  type: array
- description: The opaque reference value returned by the Adyen API during bank account login.
  name: bankAggregatorDataReference
  type: string
- description: Details about the business or nonprofit account holder. Required when creating an account holder with `legalEntity` **Business** or **NonProfit**.
  name: businessDetails
  type: object
- description: The email address of the account holder.
  name: email
  type: string
- description: The phone number of the account holder provided as a single string. It will be handled as a landline phone. **Examples:** "0031 6 11 22 33 44", "+316/1122-3344", "(0031) 611223344"
  name: fullPhoneNumber
  type: string
- description: Details about the individual account holder. Required when creating an account holder with `legalEntity` **Individual**.
  name: individualDetails
  type: object
- description: Date when you last reviewed the account holder's information, in ISO-8601 YYYY-MM-DD format. For example, **2020-01-31**.
  name: lastReviewDate
  type: string
- description: An array containing information about the account holder's [legal arrangements](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/legal-arrangements).
  name: legalArrangements
  type: array
- description: The Merchant Category Code of the account holder. > If not specified in the request, this will be derived from the platform account (which is configured by Adyen).
  name: merchantCategoryCode
  type: string
- description: A set of key and value pairs for general use by the account holder or merchant. The keys do not have specific names and may be used for storing miscellaneous data as desired. > The values being stored
  name: metadata
  type: object
- description: Array of tokenized card details associated with the account holder. For details about how you can use the tokens to pay out, refer to [Pay out to cards](https://docs.adyen.com/marketplaces-and-platfor
  name: payoutMethods
  type: array
- description: The principal business address of the account holder.
  name: principalBusinessAddress
  type: object
- description: Array of stores associated with the account holder. Required when onboarding account holders that have an Adyen [point of sale](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-
  name: storeDetails
  type: array
- description: The URL of the website of the account holder.
  name: webAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-details-schema.json
slug: notifications-account-holder-details
source_filename: notifications-account-holder-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-details-schema.json\",\n  \"title\": \"AccountHolderDetails\",\n  \"description\": \"AccountHolderDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the account holder.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"bankAccountDetails\": {\n      \"description\": \"Array of bank accounts associated with the account holder. For details about the required `bankAccountDetail` fields, see [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BankAccountDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"bankAggregatorDataReference\"\
  : {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The opaque reference value returned by the Adyen API during bank account login.\",\n      \"type\": \"string\"\n    },\n    \"businessDetails\": {\n      \"description\": \"Details about the business or nonprofit account holder.\\nRequired when creating an account holder with `legalEntity` **Business** or **NonProfit**.\",\n      \"$ref\": \"#/components/schemas/BusinessDetails\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"fullPhoneNumber\": {\n      \"description\": \"The phone number of the account holder provided as a single string. It will be handled as a landline phone.\\n**Examples:** \\\"0031 6 11 22 33 44\\\", \\\"+316/1122-3344\\\", \\\"(0031) 611223344\\\"\",\n      \"type\": \"string\"\n    },\n    \"individualDetails\": {\n      \"description\": \"Details about the individual account holder.\\nRequired when creating\
  \ an account holder with `legalEntity` **Individual**.\\n\",\n      \"$ref\": \"#/components/schemas/IndividualDetails\"\n    },\n    \"lastReviewDate\": {\n      \"description\": \"Date when you last reviewed the account holder's information, in ISO-8601 YYYY-MM-DD format. For example, **2020-01-31**.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangements\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"An array containing information about the account holder's [legal arrangements](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/legal-arrangements).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LegalArrangementDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantCategoryCode\": {\n      \"description\": \"The Merchant Category Code of the account holder.\\n> If not specified in the request, this will be derived from the platform account (which is configured by Adyen).\",\n      \"type\": \"string\"\
  \n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key and value pairs for general use by the account holder or merchant.\\nThe keys do not have specific names and may be used for storing miscellaneous data as desired.\\n> The values being stored have a maximum length of eighty (80) characters and will be truncated if necessary.\\n> Note that during an update of metadata, the omission of existing key-value pairs will result in the deletion of those key-value pairs.\",\n      \"type\": \"object\"\n    },\n    \"payoutMethods\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Array of tokenized card details associated with the account holder. For details about how you can use the tokens to pay out, refer to [Pay out to cards](https://docs.adyen.com/marketplaces-and-platforms/classic/payout-to-cards).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PayoutMethod\"\n   \
  \   },\n      \"type\": \"array\"\n    },\n    \"principalBusinessAddress\": {\n      \"description\": \"The principal business address of the account holder.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"storeDetails\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Array of stores associated with the account holder. Required when onboarding account holders that have an Adyen [point of sale](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-pos).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StoreDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"webAddress\": {\n      \"description\": \"The URL of the website of the account holder.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"address\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderDetails
---
