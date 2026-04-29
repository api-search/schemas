---
description: DescribeConnectorProfilesRequest schema from Amazon AppFlow API
layout: schema
name: DescribeConnectorProfilesRequest
properties_list:
- description: The name of the connector profile. The name is unique for each ConnectorProfile in the AWS account.
  name: connectorProfileNames
  type: array
- description: The type of connector, such as Salesforce, Marketo, and so on.
  name: connectorType
  type: string
- description: The name of the connector.
  name: connectorLabel
  type: string
- description: Specifies the maximum number of items that should be returned in the result set. The default for maxResults is 20.
  name: maxResults
  type: integer
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-connector-profiles-request-schema.json
slug: appflow-describe-connector-profiles-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-profiles-request-schema.json\",\n  \"title\": \"DescribeConnectorProfilesRequest\",\n  \"description\": \"DescribeConnectorProfilesRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"\"\n      },\n      \"example\": [\n        \"my-salesforce-profile\"\n      ],\n      \"description\": \"The name of the connector profile. The name is unique for each ConnectorProfile in the AWS account.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"The type of connector, such as Salesforce, Marketo, and so on.\"\n    },\n    \"connectorLabel\":\
  \ {\n      \"type\": \"string\",\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The name of the connector.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 20,\n      \"description\": \"Specifies the maximum number of items that should be returned in the result set. The default for maxResults is 20.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-profiles-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeConnectorProfilesRequest
---
