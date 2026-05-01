---
description: ListConnectorEntitiesResponse schema from Amazon AppFlow API
layout: schema
name: ListConnectorEntitiesResponse
properties_list:
- description: The response of ListConnectorEntities lists entities grouped by category.
  name: connectorEntityMap
  type: object
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-list-connector-entities-response-schema.json
slug: appflow-list-connector-entities-response
source_filename: appflow-list-connector-entities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connector-entities-response-schema.json\",\n  \"title\": \"ListConnectorEntitiesResponse\",\n  \"description\": \"ListConnectorEntitiesResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorEntityMap\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"$ref\": \"#/components/schemas/ConnectorEntity\"\n        }\n      },\n      \"description\": \"The response of ListConnectorEntities lists entities grouped by category.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connector-entities-response-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ListConnectorEntitiesResponse
---
