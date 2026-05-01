---
description: DescribeConnectorEntityRequest schema from Amazon AppFlow API
layout: schema
name: DescribeConnectorEntityRequest
properties_list:
- description: The entity name for that connector.
  name: connectorEntityName
  type: string
- description: The type of connector application, such as Salesforce, Marketo, and so on.
  name: connectorType
  type: string
- description: The name of the connector profile. The name is unique for each ConnectorProfile in the AWS account.
  name: connectorProfileName
  type: string
- description: The version of the API that's used by the connector.
  name: apiVersion
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-connector-entity-request-schema.json
slug: appflow-describe-connector-entity-request
source_filename: appflow-describe-connector-entity-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-entity-request-schema.json\",\n  \"title\": \"DescribeConnectorEntityRequest\",\n  \"description\": \"DescribeConnectorEntityRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorEntityName\": {\n      \"type\": \"string\",\n      \"maxLength\": 1024,\n      \"example\": \"Account\",\n      \"description\": \"The entity name for that connector.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"The type of connector application, such as Salesforce, Marketo, and so on.\"\n    },\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile. The name\
  \ is unique for each ConnectorProfile in the AWS account.\"\n    },\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v55.0\",\n      \"description\": \"The version of the API that's used by the connector.\"\n    }\n  },\n  \"required\": [\n    \"connectorEntityName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-entity-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeConnectorEntityRequest
---
