---
description: Represents a single application with a larger set of attributes than provided in the AppSummary, including Instances, Activity, Contract, Fiscal Spend, Compliance, and SSO Protocols.
layout: schema
name: AppDetails
properties_list:
- description: The unique identifier of the application.
  name: ApplicationId
  type: string
- description: The name of the application.
  name: AppName
  type: string
- description: The current status of the application.
  name: AppStatus
  type: string
- description: The name of the vendor.
  name: VendorName
  type: string
- description: Application instances.
  name: Instances
  type: array
- description: Usage activity metrics for the application.
  name: Activity
  type: object
- description: Contract details associated with the application.
  name: Contracts
  type: array
- description: Fiscal spend data for the application.
  name: FiscalSpend
  type: object
- description: Security standard compliance information.
  name: Compliance
  type: object
- description: SSO protocols supported by the application.
  name: SSOProtocols
  type: array
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/productiv-developer-app-details-schema.json
slug: productiv-developer-app-details
source_filename: productiv-developer-app-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppDetails\",\n  \"type\": \"object\",\n  \"description\": \"Represents a single application with a larger set of attributes than provided in the AppSummary, including Instances, Activity, Contract, Fiscal Spend, Compliance, and SSO Protocols.\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application.\"\n    },\n    \"AppName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"AppStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the application.\"\n    },\n    \"VendorName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the vendor.\"\n    },\n    \"Instances\": {\n      \"type\": \"array\",\n      \"description\": \"Application instances.\"\n    },\n    \"Activity\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Usage activity metrics for the application.\"\n    },\n    \"Contracts\": {\n      \"type\": \"array\",\n      \"description\": \"Contract details associated with the application.\"\n    },\n    \"FiscalSpend\": {\n      \"type\": \"object\",\n      \"description\": \"Fiscal spend data for the application.\"\n    },\n    \"Compliance\": {\n      \"type\": \"object\",\n      \"description\": \"Security standard compliance information.\"\n    },\n    \"SSOProtocols\": {\n      \"type\": \"array\",\n      \"description\": \"SSO protocols supported by the application.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/productiv-developer-app-details-schema.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: AppDetails
---
