---
description: ''
layout: schema
name: SuccessfulAuthenticationConfigurationEndpoint
properties_list:
- description: ''
  name: OrgId
  type: string
- description: ''
  name: Url
  type: string
- description: ''
  name: MobileSDK
  type: object
- description: ''
  name: LoginPage
  type: '[''string'', ''null'']'
- description: ''
  name: SamlProviders
  type: array
- description: ''
  name: AuthProviders
  type: array
- description: ''
  name: CertificateLogin
  type: '[''string'', ''null'']'
- description: ''
  name: LoginPageType
  type: string
- description: ''
  name: LoginPageTypeConfigs
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-authentication-configuration-endpoint-schema.json
slug: salesforce-successful-authentication-configuration-endpoint
source_filename: salesforce-successful-authentication-configuration-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrgId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"Url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"MobileSDK\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"UseiOSNativeBrowserForAuthentication\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"UseAndroidNativeBrowserForAuthentication\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"shareBrowserSessionIOS\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"shareBrowserSessionAndroid\": {\n          \"type\": \"boolean\",\n          \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"UseiOSNativeBrowserForAuthentication\",\n        \"UseAndroidNativeBrowserForAuthentication\",\n        \"shareBrowserSessionIOS\",\n  \
  \      \"shareBrowserSessionAndroid\"\n      ]\n    },\n    \"LoginPage\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"SamlProviders\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"AuthProviders\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CertificateLogin\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"LoginPageType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LoginPageTypeConfigs\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"OrgId\",\n    \"Url\",\n    \"MobileSDK\",\n    \"LoginPage\",\n    \"SamlProviders\",\n    \"AuthProviders\",\n    \"CertificateLogin\"\
  ,\n    \"LoginPageType\",\n    \"LoginPageTypeConfigs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulAuthenticationConfigurationEndpoint\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-authentication-configuration-endpoint-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: SuccessfulAuthenticationConfigurationEndpoint
---
