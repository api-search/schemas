---
description: Schema for an SAP API Management API Proxy, which fronts a backend service and applies policies for security, transformation, and throttling.
layout: schema
name: SAP API Management API Proxy
properties_list:
- description: Unique identifier for the API proxy
  name: name
  type: string
- description: Human-readable display title shown in the developer portal
  name: title
  type: string
- description: Detailed description of the API proxy's purpose and usage
  name: description
  type: string
- description: API version string
  name: version
  type: string
- description: Base path for routing incoming requests to this proxy
  name: basepath
  type: string
- description: Deployment status of the API proxy
  name: status
  type: string
- description: Reference to the API provider (backend system) this proxy fronts
  name: apiProviderId
  type: string
- description: Creation timestamp
  name: createdAt
  type: string
- description: Last modification timestamp
  name: modifiedAt
  type: string
provider_name: SAP API Management
provider_slug: sap-api-management
schema_file: json-schema/sap-api-management-api-proxy-schema.json
slug: sap-api-management-api-proxy
source_filename: sap-api-management-api-proxy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sap-api-management/json-schema/api-proxy.json\",\n  \"title\": \"SAP API Management API Proxy\",\n  \"description\": \"Schema for an SAP API Management API Proxy, which fronts a backend service and applies policies for security, transformation, and throttling.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"basepath\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API proxy\",\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9_-]*$\",\n      \"examples\": [\"OrderManagement\", \"customer-api-v2\"]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display title shown in the developer portal\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the API proxy's purpose and usage\"\n    },\n\
  \    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version string\",\n      \"examples\": [\"v1\", \"v2\", \"1.0\"]\n    },\n    \"basepath\": {\n      \"type\": \"string\",\n      \"description\": \"Base path for routing incoming requests to this proxy\",\n      \"examples\": [\"/orders\", \"/customers/v2\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\", \"Draft\"],\n      \"description\": \"Deployment status of the API proxy\"\n    },\n    \"apiProviderId\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the API provider (backend system) this proxy fronts\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-api-management/refs/heads/main/json-schema/sap-api-management-api-proxy-schema.json
tags:
- API Management
- Developer Portal
- Enterprise
- SAP
title: SAP API Management API Proxy
---
