---
description: AccountHolder schema from Adyen API
layout: schema
name: AccountHolder
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
- description: The unique identifier of the account holder.
  name: id
  type: string
- description: 'The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) associated with the account holder. Adyen performs a verification '
  name: legalEntityId
  type: string
- description: The ID of the account holder's primary balance account. By default, this is set to the first balance account that you create for the account holder. To assign a different balance account, send a PATCH
  name: primaryBalanceAccount
  type: string
- description: Your reference for the account holder, maximum 150 characters.
  name: reference
  type: string
- description: 'The status of the account holder. Possible values: * **Active**: The account holder is active. This is the default status when creating an account holder. * **Inactive**: The account holder is tempora'
  name: status
  type: string
- description: The [time zone](https://www.iana.org/time-zones) of the account holder. For example, **Europe/Amsterdam**. If not set, the time zone of the balance account will be used. For possible values, see the [
  name: timeZone
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-account-holder-schema.json
slug: notification-webhooks-account-holder
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-account-holder-schema.json\",\n  \"title\": \"AccountHolder\",\n  \"description\": \"AccountHolder schema from Adyen API\",\n  \"properties\": {\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the [balance platform](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balancePlatforms/{id}__queryParam_id) to which the account holder belongs. Required in the request if your API credentials can be used for multiple balance platforms.\",\n      \"type\": \"string\"\n    },\n    \"capabilities\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AccountHolderCapability\"\n      },\n      \"description\": \"Contains key-value pairs that specify the actions that an account holder can do in your platform. The key is a capability\
  \ required for your integration. For example, **issueCard** for Issuing. The value is an object containing the settings for the capability.\",\n      \"type\": \"object\"\n    },\n    \"contactDetails\": {\n      \"description\": \"Contact details of the account holder.\",\n      \"$ref\": \"#/components/schemas/ContactDetails\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the account holder, maximum 300 characters.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"legalEntityId\": {\n      \"description\": \"The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) associated with the account holder. Adyen performs a verification process against the legal entity of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"\
  primaryBalanceAccount\": {\n      \"description\": \"The ID of the account holder's primary balance account. By default, this is set to the first balance account that you create for the account holder. To assign a different balance account, send a PATCH request.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the account holder, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the account holder.\\n\\nPossible values: \\n\\n * **Active**: The account holder is active. This is the default status when creating an account holder. \\n\\n * **Inactive**: The account holder is temporarily inactive due to missing KYC details. You can set the account back to active by providing the missing KYC details. \\n\\n * **Suspended**: The account holder is permanently deactivated by Adyen. This action cannot be undone. \\n\\n* **Closed**: The account\
  \ holder is permanently deactivated by you. This action cannot be undone.\",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Inactive\",\n        \"Suspended\"\n      ],\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"description\": \"The [time zone](https://www.iana.org/time-zones) of the account holder. For example, **Europe/Amsterdam**.\\nIf not set, the time zone of the balance account will be used. For possible values, see the [list of time zone codes](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"legalEntityId\",\n    \"id\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-account-holder-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolder
---
