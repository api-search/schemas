---
description: ListConnectorEntitiesRequest schema from Amazon AppFlow API
layout: schema
name: ListConnectorEntitiesRequest
properties_list:
- description: The name of the connector profile. The name is unique for each ConnectorProfile in the AWS account.
  name: connectorProfileName
  type: string
- description: The type of connector, such as Salesforce, Marketo, and so on.
  name: connectorType
  type: string
- description: This optional parameter is specific to connector implementation. Some connectors support multiple levels or categories of entities.
  name: entitiesPath
  type: string
- description: The version of the API that's used by the connector.
  name: apiVersion
  type: string
- description: The maximum number of items that should be returned in the result set.
  name: maxResults
  type: integer
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-list-connector-entities-request-schema.json
slug: appflow-list-connector-entities-request
source_filename: appflow-list-connector-entities-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connector-entities-request-schema.json\",\n  \"title\": \"ListConnectorEntitiesRequest\",\n  \"description\": \"ListConnectorEntitiesRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile. The name is unique for each ConnectorProfile in the AWS account.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"The type of connector, such as Salesforce, Marketo, and so on.\"\n    },\n    \"entitiesPath\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"\",\n      \"description\": \"This optional\
  \ parameter is specific to connector implementation. Some connectors support multiple levels or categories of entities.\"\n    },\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v55.0\",\n      \"description\": \"The version of the API that's used by the connector.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 10000,\n      \"example\": 20,\n      \"description\": \"The maximum number of items that should be returned in the result set.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connector-entities-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ListConnectorEntitiesRequest
---
