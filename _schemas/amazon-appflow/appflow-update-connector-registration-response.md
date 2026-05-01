---
description: UpdateConnectorRegistrationResponse schema from Amazon AppFlow API
layout: schema
name: UpdateConnectorRegistrationResponse
properties_list:
- description: The ARN of the connector being updated.
  name: connectorArn
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-update-connector-registration-response-schema.json
slug: appflow-update-connector-registration-response
source_filename: appflow-update-connector-registration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-connector-registration-response-schema.json\",\n  \"title\": \"UpdateConnectorRegistrationResponse\",\n  \"description\": \"UpdateConnectorRegistrationResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:connector/MyCustomConnector\",\n      \"description\": \"The ARN of the connector being updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-connector-registration-response-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: UpdateConnectorRegistrationResponse
---
