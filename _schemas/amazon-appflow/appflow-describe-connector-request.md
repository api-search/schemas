---
description: DescribeConnectorRequest schema from Amazon AppFlow API
layout: schema
name: DescribeConnectorRequest
properties_list:
- description: The connector type, such as CUSTOMCONNECTOR, Saleforce, Marketo.
  name: connectorType
  type: string
- description: The label of the connector. The label is unique for each ConnectorRegistration in your Amazon Web Services account.
  name: connectorLabel
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-connector-request-schema.json
slug: appflow-describe-connector-request
source_filename: appflow-describe-connector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-request-schema.json\",\n  \"title\": \"DescribeConnectorRequest\",\n  \"description\": \"DescribeConnectorRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"CustomConnector\",\n      \"description\": \"The connector type, such as CUSTOMCONNECTOR, Saleforce, Marketo.\"\n    },\n    \"connectorLabel\": {\n      \"type\": \"string\",\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The label of the connector. The label is unique for each ConnectorRegistration in your Amazon Web Services account.\"\n    }\n  },\n  \"required\": [\n    \"connectorType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeConnectorRequest
---
