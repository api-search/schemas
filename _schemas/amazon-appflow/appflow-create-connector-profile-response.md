---
description: CreateConnectorProfileResponse schema from Amazon AppFlow API
layout: schema
name: CreateConnectorProfileResponse
properties_list:
- description: The Amazon Resource Name (ARN) of the connector profile.
  name: connectorProfileArn
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-create-connector-profile-response-schema.json
slug: appflow-create-connector-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-create-connector-profile-response-schema.json\",\n  \"title\": \"CreateConnectorProfileResponse\",\n  \"description\": \"CreateConnectorProfileResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:connectorprofile/my-salesforce-profile\",\n      \"description\": \"The Amazon Resource Name (ARN) of the connector profile.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-create-connector-profile-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: CreateConnectorProfileResponse
---
