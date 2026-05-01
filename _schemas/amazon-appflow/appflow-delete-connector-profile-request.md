---
description: DeleteConnectorProfileRequest schema from Amazon AppFlow API
layout: schema
name: DeleteConnectorProfileRequest
properties_list:
- description: The name of the connector profile.
  name: connectorProfileName
  type: string
- description: Indicates whether Amazon AppFlow should delete the profile, even if it is currently in use in one or more flows.
  name: forceDelete
  type: boolean
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-delete-connector-profile-request-schema.json
slug: appflow-delete-connector-profile-request
source_filename: appflow-delete-connector-profile-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-delete-connector-profile-request-schema.json\",\n  \"title\": \"DeleteConnectorProfileRequest\",\n  \"description\": \"DeleteConnectorProfileRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile.\"\n    },\n    \"forceDelete\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Indicates whether Amazon AppFlow should delete the profile, even if it is currently in use in one or more flows.\"\n    }\n  },\n  \"required\": [\n    \"connectorProfileName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-delete-connector-profile-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DeleteConnectorProfileRequest
---
