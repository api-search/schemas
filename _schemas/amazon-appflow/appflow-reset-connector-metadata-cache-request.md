---
description: ResetConnectorMetadataCacheRequest schema from Amazon AppFlow API
layout: schema
name: ResetConnectorMetadataCacheRequest
properties_list:
- description: The name of the connector profile that you want to reset cached metadata for.
  name: connectorProfileName
  type: string
- description: The type of connector to reset cached metadata for.
  name: connectorType
  type: string
- description: Use this parameter if you want to reset cached metadata about the details for an individual entity.
  name: connectorEntityName
  type: string
- description: Use this parameter only if you're resetting the cached metadata about a nested entity.
  name: entitiesPath
  type: string
- description: The API version that you specified in the connector profile that you're resetting cached metadata for.
  name: apiVersion
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-reset-connector-metadata-cache-request-schema.json
slug: appflow-reset-connector-metadata-cache-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-reset-connector-metadata-cache-request-schema.json\",\n  \"title\": \"ResetConnectorMetadataCacheRequest\",\n  \"description\": \"ResetConnectorMetadataCacheRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile that you want to reset cached metadata for.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"The type of connector to reset cached metadata for.\"\n    },\n    \"connectorEntityName\": {\n      \"type\": \"string\",\n      \"maxLength\": 1024,\n      \"example\": \"Account\",\n      \"\
  description\": \"Use this parameter if you want to reset cached metadata about the details for an individual entity.\"\n    },\n    \"entitiesPath\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"\",\n      \"description\": \"Use this parameter only if you're resetting the cached metadata about a nested entity.\"\n    },\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v55.0\",\n      \"description\": \"The API version that you specified in the connector profile that you're resetting cached metadata for.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-reset-connector-metadata-cache-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ResetConnectorMetadataCacheRequest
---
