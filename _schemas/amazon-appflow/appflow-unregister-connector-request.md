---
description: UnregisterConnectorRequest schema from Amazon AppFlow API
layout: schema
name: UnregisterConnectorRequest
properties_list:
- description: The label of the connector. The label is unique for each ConnectorRegistration in your Amazon Web Services account.
  name: connectorLabel
  type: string
- description: Indicates whether Amazon AppFlow should unregister the connector, even if it is currently in use in one or more connector profiles.
  name: forceDelete
  type: boolean
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-unregister-connector-request-schema.json
slug: appflow-unregister-connector-request
source_filename: appflow-unregister-connector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-unregister-connector-request-schema.json\",\n  \"title\": \"UnregisterConnectorRequest\",\n  \"description\": \"UnregisterConnectorRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorLabel\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The label of the connector. The label is unique for each ConnectorRegistration in your Amazon Web Services account.\"\n    },\n    \"forceDelete\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Indicates whether Amazon AppFlow should unregister the connector, even if it is currently in use in one or more connector profiles.\"\n    }\n  },\n  \"required\": [\n    \"connectorLabel\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-unregister-connector-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: UnregisterConnectorRequest
---
