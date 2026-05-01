---
description: DescribeConnectorResponse schema from Amazon AppFlow API
layout: schema
name: DescribeConnectorResponse
properties_list:
- description: Configuration info of all the connectors that the user requested.
  name: connectorConfiguration
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-connector-response-schema.json
slug: appflow-describe-connector-response
source_filename: appflow-describe-connector-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-response-schema.json\",\n  \"title\": \"DescribeConnectorResponse\",\n  \"description\": \"DescribeConnectorResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"canUseAsSource\": {\n          \"type\": \"boolean\",\n          \"example\": true,\n          \"description\": \"Specifies whether the connector can be used as a source.\"\n        },\n        \"canUseAsDestination\": {\n          \"type\": \"boolean\",\n          \"example\": true,\n          \"description\": \"Specifies whether the connector can be used as a destination.\"\n        },\n        \"connectorArn\": {\n          \"type\": \"string\",\n          \"example\": \"arn:aws:appflow:us-east-1:123456789012:connector/MyCustomConnector\"\
  ,\n          \"description\": \"The Amazon Resource Name (ARN) for the registered connector.\"\n        },\n        \"connectorLabel\": {\n          \"type\": \"string\",\n          \"example\": \"MyCustomConnector\",\n          \"description\": \"The label used for registering the connector.\"\n        },\n        \"connectorDescription\": {\n          \"type\": \"string\",\n          \"example\": \"My custom connector\",\n          \"description\": \"A description about the connector.\"\n        },\n        \"connectorOwner\": {\n          \"type\": \"string\",\n          \"example\": \"123456789012\",\n          \"description\": \"The owner of the connector.\"\n        },\n        \"connectorVersion\": {\n          \"type\": \"string\",\n          \"example\": \"1.0\",\n          \"description\": \"The connector version.\"\n        },\n        \"connectorModes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\": \"\
  \"\n          },\n          \"example\": [\n            \"CLOUD\"\n          ]\n        }\n      },\n      \"description\": \"Configuration info of all the connectors that the user requested.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-response-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeConnectorResponse
---
