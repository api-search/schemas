---
description: Represents a single application with detailed attributes including Instances, Activity, Contract, Fiscal Spend, Compliance, and SSO Protocols.
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
schema_file: json-schema/app-details.json
slug: app-details
source_json: "{\n  \"$id\": \"app-details.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppDetails\",\n  \"description\": \"Represents a single application with detailed attributes including Instances, Activity, Contract, Fiscal Spend, Compliance, and SSO Protocols.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application.\"\n    },\n    \"AppName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"AppStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the application.\"\n    },\n    \"VendorName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the vendor.\"\n    },\n    \"Instances\": {\n      \"type\": \"array\",\n      \"description\": \"Application instances.\",\n      \"items\": {\n        \"type\": \"object\",\n  \
  \      \"properties\": {\n          \"instanceId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the instance.\"\n          },\n          \"instanceName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the instance.\"\n          }\n        }\n      }\n    },\n    \"Activity\": {\n      \"type\": \"object\",\n      \"description\": \"Usage activity metrics for the application.\",\n      \"properties\": {\n        \"totalUsers\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of users.\"\n        },\n        \"activeUsers\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of active users.\"\n        },\n        \"lastActivityDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The date of last activity.\"\n        }\n      }\n    },\n    \"Contracts\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Contract details associated with the application.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"contractId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the contract.\"\n          },\n          \"startDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\",\n            \"description\": \"The start date of the contract.\"\n          },\n          \"endDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\",\n            \"description\": \"The end date of the contract.\"\n          },\n          \"totalValue\": {\n            \"type\": \"number\",\n            \"description\": \"The total value of the contract.\"\n          }\n        }\n      }\n    },\n    \"FiscalSpend\": {\n      \"type\": \"object\",\n      \"description\": \"Fiscal spend data for the application.\",\n      \"properties\": {\n        \"totalSpend\": {\n          \"type\"\
  : \"number\",\n          \"description\": \"Total spend amount.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"The currency code.\"\n        }\n      }\n    },\n    \"Compliance\": {\n      \"type\": \"object\",\n      \"description\": \"Security standard compliance information.\",\n      \"properties\": {\n        \"standards\": {\n          \"type\": \"array\",\n          \"description\": \"List of compliance standards met.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"SSOProtocols\": {\n      \"type\": \"array\",\n      \"description\": \"SSO protocols supported by the application.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/app-details.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: AppDetails
---
