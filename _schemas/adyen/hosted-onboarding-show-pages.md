---
description: ShowPages schema from Adyen API
layout: schema
name: ShowPages
properties_list:
- description: Indicates whether the page with bank account details must be shown. Defaults to **true**.
  name: bankDetailsSummaryPage
  type: boolean
- description: Indicates whether the bank check instant verification' details must be shown. Defaults to **true**.
  name: bankVerificationPage
  type: boolean
- description: Indicates whether the page with the company's or organization's details must be shown. Defaults to **true**.
  name: businessDetailsSummaryPage
  type: boolean
- description: Indicates whether the checks overview page must be shown. Defaults to **false**.
  name: checksOverviewPage
  type: boolean
- description: Indicates whether the page with the individual's details must be shown. Defaults to **true**.
  name: individualDetailsSummaryPage
  type: boolean
- description: Indicates whether the page with the legal arrangements' details must be shown. Defaults to **true**.
  name: legalArrangementsDetailsSummaryPage
  type: boolean
- description: Indicates whether the page to manually add bank account' details must be shown. Defaults to **true**.
  name: manualBankAccountPage
  type: boolean
- description: Indicates whether the page with the shareholders' details must be shown. Defaults to **true**.
  name: shareholderDetailsSummaryPage
  type: boolean
- description: Indicates whether the welcome page must be shown. Defaults to **false**.
  name: welcomePage
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/hosted-onboarding-show-pages-schema.json
slug: hosted-onboarding-show-pages
source_filename: hosted-onboarding-show-pages-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-show-pages-schema.json\",\n  \"title\": \"ShowPages\",\n  \"description\": \"ShowPages schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankDetailsSummaryPage\": {\n      \"description\": \"Indicates whether the page with bank account details must be shown. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"bankVerificationPage\": {\n      \"description\": \"Indicates whether the bank check instant verification' details must be shown. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"businessDetailsSummaryPage\": {\n      \"description\": \"Indicates whether the page with the company's or organization's details must be shown. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"checksOverviewPage\": {\n      \"description\"\
  : \"Indicates whether the checks overview page must be shown. Defaults to **false**.\",\n      \"type\": \"boolean\"\n    },\n    \"individualDetailsSummaryPage\": {\n      \"description\": \"Indicates whether the page with the individual's details must be shown. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"legalArrangementsDetailsSummaryPage\": {\n      \"description\": \"Indicates whether the page with the legal arrangements' details must be shown. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"manualBankAccountPage\": {\n      \"description\": \"Indicates whether the page to manually add bank account' details must be shown. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"shareholderDetailsSummaryPage\": {\n      \"description\": \"Indicates whether the page with the shareholders' details must be shown. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"welcomePage\": {\n      \"description\": \"Indicates\
  \ whether the welcome page must be shown. Defaults to **false**.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-show-pages-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ShowPages
---
