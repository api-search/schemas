---
description: Represents a Microsoft Purview account resource managed through Azure Resource Manager.
layout: schema
name: Microsoft Purview Account
properties_list:
- description: The Azure resource ID
  name: id
  type: string
- description: The name of the Purview account
  name: name
  type: string
- description: The resource type (Microsoft.Purview/accounts)
  name: type
  type: string
- description: The Azure region where the account is deployed
  name: location
  type: string
- description: Resource tags
  name: tags
  type: object
- description: The managed identity for the account
  name: identity
  type: object
- description: The SKU of the account
  name: sku
  type: object
- description: Account properties
  name: properties
  type: object
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-account-schema.json
slug: microsoft-purview-account
source_filename: microsoft-purview-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-account-schema.json\",\n  \"title\": \"Microsoft Purview Account\",\n  \"description\": \"Represents a Microsoft Purview account resource managed through Azure Resource Manager.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Azure resource ID\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Purview account\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type (Microsoft.Purview/accounts)\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The Azure region where the account is deployed\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Resource tags\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"identity\": {\n      \"type\": \"object\",\n      \"description\": \"The managed identity for the account\",\n      \"properties\": {\n        \"principalId\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"tenantId\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"None\", \"SystemAssigned\", \"UserAssigned\"]\n        }\n      }\n    },\n    \"sku\": {\n      \"type\": \"object\",\n      \"description\": \"The SKU of the account\",\n      \"properties\": {\n        \"capacity\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"enum\": [\"Standard\"]\n        }\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Account properties\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"The current provisioning state\",\n          \"enum\": [\"Unknown\", \"Creating\", \"Moving\", \"Deleting\", \"SoftDeleting\", \"SoftDeleted\", \"Failed\", \"Succeeded\", \"Canceled\"],\n          \"readOnly\": true\n        },\n        \"publicNetworkAccess\": {\n          \"type\": \"string\",\n          \"description\": \"Whether public network access is enabled\",\n          \"enum\": [\"NotSpecified\", \"Enabled\", \"Disabled\"]\n        },\n        \"managedResourceGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"The managed resource group name\"\n        },\n        \"endpoints\": {\n          \"type\": \"object\",\n          \"description\": \"The service endpoints\",\n          \"readOnly\": true,\n          \"properties\": {\n            \"catalog\": {\n              \"type\": \"string\",\n           \
  \   \"description\": \"The catalog endpoint URL\"\n            },\n            \"guardian\": {\n              \"type\": \"string\",\n              \"description\": \"The guardian endpoint URL\"\n            },\n            \"scan\": {\n              \"type\": \"string\",\n              \"description\": \"The scan endpoint URL\"\n            }\n          }\n        },\n        \"friendlyName\": {\n          \"type\": \"string\",\n          \"description\": \"The friendly name of the account\",\n          \"readOnly\": true\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true\n        },\n        \"createdBy\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        }\n      }\n    }\n  },\n  \"required\": [\"location\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-account-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Account
---
