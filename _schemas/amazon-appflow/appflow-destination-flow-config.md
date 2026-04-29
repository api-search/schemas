---
description: DestinationFlowConfig schema from Amazon AppFlow API
layout: schema
name: DestinationFlowConfig
properties_list:
- description: The type of connector used as a destination.
  name: connectorType
  type: string
- description: The API version that the destination connector uses.
  name: apiVersion
  type: string
- description: The name of the connector profile.
  name: connectorProfileName
  type: string
- description: This stores the information that is required to query a particular connector.
  name: destinationConnectorProperties
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-destination-flow-config-schema.json
slug: appflow-destination-flow-config
source_filename: appflow-destination-flow-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-destination-flow-config-schema.json\",\n  \"title\": \"DestinationFlowConfig\",\n  \"description\": \"DestinationFlowConfig schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"S3\",\n      \"description\": \"The type of connector used as a destination.\"\n    },\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"example\": \"2006-03-01\",\n      \"description\": \"The API version that the destination connector uses.\"\n    },\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"example\": \"my-s3-profile\",\n      \"description\": \"The name of the connector profile.\"\n    },\n    \"destinationConnectorProperties\": {\n      \"type\": \"object\",\n      \"example\"\
  : {\n        \"S3\": {\n          \"bucketName\": \"my-data-bucket\",\n          \"bucketPrefix\": \"appflow/salesforce/accounts\"\n        }\n      },\n      \"description\": \"This stores the information that is required to query a particular connector.\"\n    }\n  },\n  \"required\": [\n    \"connectorType\",\n    \"destinationConnectorProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-destination-flow-config-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DestinationFlowConfig
---
