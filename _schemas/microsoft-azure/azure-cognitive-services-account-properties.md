---
description: Properties of Cognitive Services account.
layout: schema
name: AccountProperties
properties_list:
- description: The status of the cognitive services account at the time of the operation.
  name: provisioningState
  type: string
- description: Endpoint of the created account.
  name: endpoint
  type: string
- description: Dictionary of endpoints for the cognitive services account.
  name: endpoints
  type: object
- description: The capabilities of the cognitive services account.
  name: capabilities
  type: array
- description: Whether this account has been migrated.
  name: isMigrated
  type: boolean
- description: The date of creation.
  name: dateCreated
  type: string
- description: Optional subdomain name used for token-based authentication.
  name: customSubDomainName
  type: string
- description: Whether or not public endpoint access is allowed.
  name: publicNetworkAccess
  type: string
- description: Whether to disable local authentication methods.
  name: disableLocalAuth
  type: boolean
- description: Whether to restrict outbound network access.
  name: restrictOutboundNetworkAccess
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-account-properties-schema.json
slug: azure-cognitive-services-account-properties
source_filename: azure-cognitive-services-account-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of Cognitive Services account.\",\n  \"properties\": {\n    \"provisioningState\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the cognitive services account at the time of the operation.\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint of the created account.\"\n    },\n    \"endpoints\": {\n      \"type\": \"object\",\n      \"description\": \"Dictionary of endpoints for the cognitive services account.\"\n    },\n    \"capabilities\": {\n      \"type\": \"array\",\n      \"description\": \"The capabilities of the cognitive services account.\"\n    },\n    \"isMigrated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this account has been migrated.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The date of creation.\"\n    },\n    \"customSubDomainName\": {\n      \"type\": \"string\",\n      \"description\": \"Optional subdomain name used for token-based authentication.\"\n    },\n    \"publicNetworkAccess\": {\n      \"type\": \"string\",\n      \"description\": \"Whether or not public endpoint access is allowed.\"\n    },\n    \"disableLocalAuth\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable local authentication methods.\"\n    },\n    \"restrictOutboundNetworkAccess\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to restrict outbound network access.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-account-properties-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: AccountProperties
---
