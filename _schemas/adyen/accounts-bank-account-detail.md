---
description: BankAccountDetail schema from Adyen API
layout: schema
name: BankAccountDetail
properties_list:
- description: The bank account number (without separators). >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field
  name: accountNumber
  type: string
- description: 'The type of bank account. Only applicable to bank accounts held in the USA. The permitted values are: `checking`, `savings`. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-pl'
  name: accountType
  type: string
- description: The name of the bank account.
  name: bankAccountName
  type: string
- description: Merchant reference to the bank account.
  name: bankAccountReference
  type: string
- description: 'The unique identifier (UUID) of the Bank Account. >If, during an account holder create or update request, this field is left blank (but other fields provided), a new Bank Account will be created with '
  name: bankAccountUUID
  type: string
- description: The bank identifier code. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.
  name: bankBicSwift
  type: string
- description: The city in which the bank branch is located. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field
  name: bankCity
  type: string
- description: The bank code of the banking institution with which the bank account is registered. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/requ
  name: bankCode
  type: string
- description: The name of the banking institution with which the bank account is held. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-inform
  name: bankName
  type: string
- description: 'The branch code of the branch under which the bank account is registered. The value to be specified in this parameter depends on the country of the bank account: * United States - Routing number * Uni'
  name: branchCode
  type: string
- description: The check code of the bank account. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requireme
  name: checkCode
  type: string
- description: The two-letter country code in which the bank account is registered. >The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL'). >Refer to [Required information](https://docs.adyen.com
  name: countryCode
  type: string
- description: The currency in which the bank account deals. >The permitted currency codes are defined in ISO-4217 (e.g. 'EUR').
  name: currencyCode
  type: string
- description: The international bank account number. >The IBAN standard is defined in ISO-13616. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/requi
  name: iban
  type: string
- description: The city of residence of the bank account owner. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on fi
  name: ownerCity
  type: string
- description: The country code of the country of residence of the bank account owner. >The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL'). >Refer to [Required information](https://docs.adyen.
  name: ownerCountryCode
  type: string
- description: The date of birth of the bank account owner. The date should be in ISO-8601 format yyyy-mm-dd (e.g. 2000-01-31).
  name: ownerDateOfBirth
  type: string
- description: The house name or number of the residence of the bank account owner. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-informatio
  name: ownerHouseNumberOrName
  type: string
- description: The name of the bank account owner. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requireme
  name: ownerName
  type: string
- description: The country code of the country of nationality of the bank account owner. >The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL'). >Refer to [Required information](https://docs.adye
  name: ownerNationality
  type: string
- description: The postal code of the residence of the bank account owner. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for de
  name: ownerPostalCode
  type: string
- description: The state of residence of the bank account owner. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on f
  name: ownerState
  type: string
- description: The street name of the residence of the bank account owner. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for de
  name: ownerStreet
  type: string
- description: If set to true, the bank account is a primary account.
  name: primaryAccount
  type: boolean
- description: The tax ID number. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.
  name: taxId
  type: string
- description: The URL to be used for bank account verification. This may be generated on bank account creation. >Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verificatio
  name: urlForVerification
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-bank-account-detail-schema.json
slug: accounts-bank-account-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-bank-account-detail-schema.json\",\n  \"title\": \"BankAccountDetail\",\n  \"description\": \"BankAccountDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The bank account number (without separators).\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"accountType\": {\n      \"description\": \"The type of bank account.\\nOnly applicable to bank accounts held in the USA.\\nThe permitted values are: `checking`, `savings`.\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details\
  \ on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountName\": {\n      \"description\": \"The name of the bank account.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountReference\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Merchant reference to the bank account.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUID\": {\n      \"description\": \"The unique identifier (UUID) of the Bank Account.\\n>If, during an account holder create or update request, this field is left blank (but other fields provided), a new Bank Account will be created with a procedurally-generated UUID.\\n\\n>If, during an account holder create request, a UUID is provided, the creation of the Bank Account will fail while the creation of the account holder will continue.\\n\\n>If, during an account holder update request, a UUID that is not correlated with an existing Bank Account is provided, the update of the account holder will fail.\\n\\n>If, during\
  \ an account holder update request, a UUID that is correlated with an existing Bank Account is provided, the existing Bank Account will be updated.\\n\",\n      \"type\": \"string\"\n    },\n    \"bankBicSwift\": {\n      \"description\": \"The bank identifier code.\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"bankCity\": {\n      \"description\": \"The city in which the bank branch is located.\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"bankCode\": {\n      \"description\": \"The bank code of the banking institution with which the bank account is registered.\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information)\
  \ for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"bankName\": {\n      \"description\": \"The name of the banking institution with which the bank account is held.\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"branchCode\": {\n      \"description\": \"The branch code of the branch under which the bank account is registered. The value to be specified in this parameter depends on the country of the bank account:\\n* United States - Routing number\\n* United Kingdom - Sort code\\n* Germany - Bankleitzahl\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"checkCode\": {\n      \"description\": \"The check code of the bank account.\\\
  n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"description\": \"The two-letter country code in which the bank account is registered.\\n>The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL').\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"description\": \"The currency in which the bank account deals.\\n>The permitted currency codes are defined in ISO-4217 (e.g. 'EUR').\\n\",\n      \"type\": \"string\"\n    },\n    \"iban\": {\n      \"description\": \"The international bank account number.\\n>The IBAN standard is defined in ISO-13616.\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information)\
  \ for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerCity\": {\n      \"description\": \"The city of residence of the bank account owner.\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerCountryCode\": {\n      \"description\": \"The country code of the country of residence of the bank account owner.\\n>The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL').\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerDateOfBirth\": {\n      \"deprecated\": true,\n      \"description\": \"The date of birth of the bank account owner.\\nThe date should be in ISO-8601 format yyyy-mm-dd (e.g. 2000-01-31).\"\
  ,\n      \"type\": \"string\"\n    },\n    \"ownerHouseNumberOrName\": {\n      \"description\": \"The house name or number of the residence of the bank account owner.\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"description\": \"The name of the bank account owner.\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerNationality\": {\n      \"description\": \"The country code of the country of nationality of the bank account owner.\\n>The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL').\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information)\
  \ for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerPostalCode\": {\n      \"description\": \"The postal code of the residence of the bank account owner.\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerState\": {\n      \"description\": \"The state of residence of the bank account owner.\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"ownerStreet\": {\n      \"description\": \"The street name of the residence of the bank account owner.\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n     \
  \ \"type\": \"string\"\n    },\n    \"primaryAccount\": {\n      \"description\": \"If set to true, the bank account is a primary account.\",\n      \"type\": \"boolean\"\n    },\n    \"taxId\": {\n      \"description\": \"The tax ID number.\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    },\n    \"urlForVerification\": {\n      \"description\": \"The URL to be used for bank account verification.\\nThis may be generated on bank account creation.\\n\\n>Refer to [Required information](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/required-information) for details on field requirements.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-bank-account-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccountDetail
---
