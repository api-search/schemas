---
description: OnboardingLinkInfo schema from Adyen API
layout: schema
name: OnboardingLinkInfo
properties_list:
- description: The language that will be used for the page, specified by a combination of two letter [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language and [ISO 3166-1 alpha-2](https://en.wi
  name: locale
  type: string
- description: The URL where the user is redirected after they complete hosted onboarding.
  name: redirectUrl
  type: string
- description: 'Boolean key-value pairs indicating the settings for the hosted onboarding page. The keys are the settings. Possible keys: By default, these values are set to **true**. Set to **false** to not allow th'
  name: settings
  type: object
- description: The unique identifier of the hosted onboarding theme.
  name: themeId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-onboarding-link-info-schema.json
slug: legal-entity-onboarding-link-info
source_filename: legal-entity-onboarding-link-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-link-info-schema.json\",\n  \"title\": \"OnboardingLinkInfo\",\n  \"description\": \"OnboardingLinkInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locale\": {\n      \"description\": \"The language that will be used for the page, specified by a combination of two letter [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language and [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country codes. See [possible values](https://docs.adyen.com/marketplaces-and-platforms/collect-verification-details/hosted#supported-languages). \\n\\nIf not specified in the request or if the language is not supported, the page uses the browser language. If the browser language is not supported, the page uses **en-US** by default.\",\n   \
  \   \"type\": \"string\"\n    },\n    \"redirectUrl\": {\n      \"description\": \"The URL where the user is redirected after they complete hosted onboarding.\",\n      \"type\": \"string\"\n    },\n    \"settings\": {\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      },\n      \"description\": \"Boolean key-value pairs indicating the settings for the hosted onboarding page. The keys are the settings.\\n\\nPossible keys:\\n\\nBy default, these values are set to **true**. Set to **false** to not allow the action.\\n\\n- **changeLegalEntityType**: The user can change their legal entity type.\\n\\n- **editPrefilledCountry**: The user can change the country of their legal entity's address, for example the registered address of an organization.\\n\\nBy default, these values are set to **false**. Set to **true** to allow the action.\\n\\n- **allowBankAccountFormatSelection**: The user can select the format for their payout account if applicable.\\n\\n- **allowIntraRegionCrossBorderPayout**:\
  \ The user can select a payout account in a different EU/EEA country than the country of their legal entity.\\n\\nBy default, these value are set to **false**. Set the following values to **true** to require the user to sign PCI questionnaires based on their sales channels. The user must sign PCI questionnaires for all relevant sales channels.\\n\\n- **requirePciSignEcommerce**\\n\\n- **requirePciSignPos**\\n\\n- **requirePciSignEcomMoto**\\n\\n- **requirePciSignPosMoto**\\n\\n\",\n      \"type\": \"object\"\n    },\n    \"themeId\": {\n      \"description\": \"The unique identifier of the hosted onboarding theme.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-onboarding-link-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OnboardingLinkInfo
---
