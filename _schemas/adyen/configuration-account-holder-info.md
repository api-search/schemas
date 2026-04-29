---
description: AccountHolderInfo schema from Adyen API
layout: schema
name: AccountHolderInfo
properties_list:
- description: 'The unique identifier of the [balance platform](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balancePlatforms/{id}__queryParam_id) to which the account holder belongs. Required in '
  name: balancePlatform
  type: string
- description: Contains key-value pairs that specify the actions that an account holder can do in your platform. The key is a capability required for your integration. For example, **issueCard** for Issuing. The val
  name: capabilities
  type: object
- description: Contact details of the account holder.
  name: contactDetails
  type: object
- description: Your description for the account holder, maximum 300 characters.
  name: description
  type: string
- description: The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id) associated with the account holder. Adyen performs a verificatio
  name: legalEntityId
  type: string
- description: A set of key and value pairs for general use. The keys do not have specific names and may be used for storing miscellaneous data as desired. > Note that during an update of metadata, the omission of e
  name: metadata
  type: object
- description: The unique identifier of the migrated account holder in the classic integration.
  name: migratedAccountHolderCode
  type: string
- description: Your reference for the account holder, maximum 150 characters.
  name: reference
  type: string
- description: The time zone of the account holder. For example, **Europe/Amsterdam**. Defaults to the time zone of the balance platform if no time zone is set. For possible values, see the [list of time zone codes]
  name: timeZone
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-account-holder-info-schema.json
slug: configuration-account-holder-info
source_filename: configuration-account-holder-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-account-holder-info-schema.json\",\n  \"title\": \"AccountHolderInfo\",\n  \"description\": \"AccountHolderInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the [balance platform](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balancePlatforms/{id}__queryParam_id) to which the account holder belongs. Required in the request if your API credentials can be used for multiple balance platforms.\",\n      \"type\": \"string\"\n    },\n    \"capabilities\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AccountHolderCapability\"\n      },\n      \"description\": \"Contains key-value pairs that specify the actions that an account holder can do in your platform.\
  \ The key is a capability required for your integration. For example, **issueCard** for Issuing. The value is an object containing the settings for the capability.\",\n      \"type\": \"object\"\n    },\n    \"contactDetails\": {\n      \"deprecated\": true,\n      \"description\": \"Contact details of the account holder.\",\n      \"$ref\": \"#/components/schemas/ContactDetails\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the account holder, maximum 300 characters.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"legalEntityId\": {\n      \"description\": \"The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id) associated with the account holder. Adyen performs a verification process against the legal entity of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"\
  string\"\n      },\n      \"description\": \"A set of key and value pairs for general use.\\nThe keys do not have specific names and may be used for storing miscellaneous data as desired.\\n> Note that during an update of metadata, the omission of existing key-value pairs will result in the deletion of those key-value pairs.\",\n      \"type\": \"object\"\n    },\n    \"migratedAccountHolderCode\": {\n      \"description\": \"The unique identifier of the migrated account holder in the classic integration.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the account holder, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"description\": \"The time zone of the account holder. For example, **Europe/Amsterdam**.\\nDefaults to the time zone of the balance platform if no time zone is set. For possible values, see the [list of time zone codes](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"legalEntityId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-account-holder-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderInfo
---
