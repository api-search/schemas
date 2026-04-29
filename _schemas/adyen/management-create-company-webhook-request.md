---
description: CreateCompanyWebhookRequest schema from Adyen API
layout: schema
name: CreateCompanyWebhookRequest
properties_list:
- description: 'Indicates if expired SSL certificates are accepted. Default value: **false**.'
  name: acceptsExpiredCertificate
  type: boolean
- description: 'Indicates if self-signed SSL certificates are accepted. Default value: **false**.'
  name: acceptsSelfSignedCertificate
  type: boolean
- description: 'Indicates if untrusted SSL certificates are accepted. Default value: **false**.'
  name: acceptsUntrustedRootCertificate
  type: boolean
- description: Indicates if the webhook configuration is active. The field must be **true** for us to send webhooks about events related an account.
  name: active
  type: boolean
- description: Additional shopper and transaction information to be included in your [standard notifications](https://docs.adyen.com/development-resources/webhooks/understand-notifications#event-codes). Find out mor
  name: additionalSettings
  type: object
- description: 'Format or protocol for receiving webhooks. Possible values: * **soap** * **http** * **json**'
  name: communicationFormat
  type: string
- description: Your description for this webhook configuration.
  name: description
  type: string
- description: 'SSL version to access the public webhook URL specified in the `url` field. Possible values: * **TLSv1.3** * **TLSv1.2** * **HTTP** - Only allowed on Test environment. If not specified, the webhook wil'
  name: encryptionProtocol
  type: string
- description: 'Shows how merchant accounts are filtered when configuring the webhook. Possible values: * **allAccounts** : Includes all merchant accounts, and does not require specifying `filterMerchantAccounts`. * '
  name: filterMerchantAccountType
  type: string
- description: A list of merchant account names that are included or excluded from receiving the webhook. Inclusion or exclusion is based on the value defined for `filterMerchantAccountType`. Required if `filterMerc
  name: filterMerchantAccounts
  type: array
- description: 'Network type for Terminal API notification webhooks. Possible values: * **public** * **local** Default Value: **public**.'
  name: networkType
  type: string
- description: Password to access the webhook URL.
  name: password
  type: string
- description: 'Indicates if the SOAP action header needs to be populated. Default value: **false**. Only applies if `communicationFormat`: **soap**.'
  name: populateSoapActionHeader
  type: boolean
- description: 'The type of webhook that is being created. Possible values are: - **standard** - **account-settings-notification** - **banktransfer-notification** - **boletobancario-notification** - **directdebit-not'
  name: type
  type: string
- description: Public URL where webhooks will be sent, for example **https://www.domain.com/webhook-endpoint**.
  name: url
  type: string
- description: Username to access the webhook URL.
  name: username
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-create-company-webhook-request-schema.json
slug: management-create-company-webhook-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-company-webhook-request-schema.json\",\n  \"title\": \"CreateCompanyWebhookRequest\",\n  \"description\": \"CreateCompanyWebhookRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptsExpiredCertificate\": {\n      \"description\": \"Indicates if expired SSL certificates are accepted. Default value: **false**.\",\n      \"type\": \"boolean\"\n    },\n    \"acceptsSelfSignedCertificate\": {\n      \"description\": \"Indicates if self-signed SSL certificates are accepted. Default value: **false**.\",\n      \"type\": \"boolean\"\n    },\n    \"acceptsUntrustedRootCertificate\": {\n      \"description\": \"Indicates if untrusted SSL certificates are accepted. Default value: **false**.\",\n      \"type\": \"boolean\"\n    },\n    \"active\": {\n      \"description\"\
  : \"Indicates if the webhook configuration is active. The field must be **true** for us to send webhooks about events related an account.\",\n      \"type\": \"boolean\"\n    },\n    \"additionalSettings\": {\n      \"description\": \"Additional shopper and transaction information to be included in your [standard notifications](https://docs.adyen.com/development-resources/webhooks/understand-notifications#event-codes). Find out more about the available [additional settings](https://docs.adyen.com/development-resources/webhooks/additional-settings).\",\n      \"$ref\": \"#/components/schemas/AdditionalSettings\"\n    },\n    \"communicationFormat\": {\n      \"description\": \"Format or protocol for receiving webhooks. Possible values:\\n* **soap**\\n* **http**\\n* **json** \",\n      \"enum\": [\n        \"http\",\n        \"json\",\n        \"soap\"\n      ],\n      \"example\": \"soap\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Your description\
  \ for this webhook configuration.\",\n      \"type\": \"string\"\n    },\n    \"encryptionProtocol\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"SSL version to access the public webhook URL specified in the `url` field. Possible values:\\n* **TLSv1.3**\\n* **TLSv1.2**\\n* **HTTP** - Only allowed on Test environment.\\n\\nIf not specified, the webhook will use `sslVersion`: **TLSv1.2**.\",\n      \"enum\": [\n        \"HTTP\",\n        \"TLSv1.2\",\n        \"TLSv1.3\"\n      ],\n      \"example\": \"TLSv1.2\",\n      \"type\": \"string\"\n    },\n    \"filterMerchantAccountType\": {\n      \"description\": \"Shows how merchant accounts are filtered when configuring the webhook. \\n\\nPossible values:\\n*  **allAccounts** : Includes all merchant accounts, and does not require specifying `filterMerchantAccounts`.\\n*  **includeAccounts** : The webhook is configured for the merchant accounts listed in `filterMerchantAccounts`.\\n*  **excludeAccounts** : The webhook is\
  \ not configured for the merchant accounts listed in `filterMerchantAccounts`.\\n\\n\",\n      \"enum\": [\n        \"allAccounts\",\n        \"excludeAccounts\",\n        \"includeAccounts\"\n      ],\n      \"type\": \"string\"\n    },\n    \"filterMerchantAccounts\": {\n      \"description\": \"A list of merchant account names that are included or excluded from receiving the webhook. Inclusion or exclusion is based on the value defined for `filterMerchantAccountType`.\\n\\nRequired if `filterMerchantAccountType` is either:\\n* **includeAccounts**\\n* **excludeAccounts**\\n\\nNot needed for `filterMerchantAccountType`: **allAccounts**.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"networkType\": {\n      \"description\": \"Network type for Terminal API notification webhooks. Possible values:\\n* **public**\\n* **local**\\n\\nDefault Value: **public**.\",\n      \"enum\": [\n        \"local\",\n        \"public\"\n      ],\n \
  \     \"type\": \"string\"\n    },\n    \"password\": {\n      \"description\": \"Password to access the webhook URL.\",\n      \"type\": \"string\"\n    },\n    \"populateSoapActionHeader\": {\n      \"description\": \"Indicates if the SOAP action header needs to be populated. Default value: **false**.\\n\\nOnly applies if `communicationFormat`: **soap**.\",\n      \"type\": \"boolean\"\n    },\n    \"type\": {\n      \"description\": \"The type of webhook that is being created. Possible values are:\\n\\n- **standard**\\n- **account-settings-notification**\\n- **banktransfer-notification**\\n- **boletobancario-notification**\\n- **directdebit-notification**\\n- **ach-notification-of-change-notification**\\n- **pending-notification**\\n- **ideal-notification**\\n- **ideal-pending-notification**\\n- **report-notification**\\n- **rreq-notification**\\n\\nFind out more about [standard notification webhooks](https://docs.adyen.com/development-resources/webhooks/understand-notifications#event-codes)\
  \ and [other types of notifications](https://docs.adyen.com/development-resources/webhooks/understand-notifications#other-notifications).\",\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\": \"Public URL where webhooks will be sent, for example **https://www.domain.com/webhook-endpoint**.\",\n      \"example\": \"http://www.adyen.com\",\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"description\": \"Username to access the webhook URL.\",\n      \"maxLength\": 255,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"url\",\n    \"active\",\n    \"communicationFormat\",\n    \"type\",\n    \"filterMerchantAccountType\",\n    \"filterMerchantAccounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-company-webhook-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateCompanyWebhookRequest
---
