---
description: DescribeConnectorProfilesResponse schema from Amazon AppFlow API
layout: schema
name: DescribeConnectorProfilesResponse
properties_list:
- description: Returns information about the connector profiles associated with the flow.
  name: connectorProfileDetails
  type: array
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-connector-profiles-response-schema.json
slug: appflow-describe-connector-profiles-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-profiles-response-schema.json\",\n  \"title\": \"DescribeConnectorProfilesResponse\",\n  \"description\": \"DescribeConnectorProfilesResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileDetails\": {\n      \"type\": \"array\",\n      \"items\": {},\n      \"description\": \"Returns information about the connector profiles associated with the flow.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connector-profiles-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeConnectorProfilesResponse
---
