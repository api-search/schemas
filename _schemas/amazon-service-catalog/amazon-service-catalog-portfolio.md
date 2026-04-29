---
description: Information about a Service Catalog portfolio.
layout: schema
name: Portfolio
properties_list:
- description: The portfolio identifier.
  name: Id
  type: string
- description: The ARN assigned to the portfolio.
  name: ARN
  type: string
- description: The name to use for display purposes.
  name: DisplayName
  type: string
- description: The description of the portfolio.
  name: Description
  type: string
- description: The UTC time stamp of the creation time.
  name: CreatedTime
  type: string
- description: The name of the portfolio provider.
  name: ProviderName
  type: string
provider_name: Amazon Service Catalog
provider_slug: amazon-service-catalog
schema_file: json-schema/amazon-service-catalog-portfolio-schema.json
slug: amazon-service-catalog-portfolio
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-service-catalog/refs/heads/main/json-schema/amazon-service-catalog-portfolio-schema.json\",\n  \"title\": \"Portfolio\",\n  \"description\": \"Information about a Service Catalog portfolio.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The portfolio identifier.\",\n      \"example\": \"port-a1b2c3d4\"\n    },\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN assigned to the portfolio.\",\n      \"example\": \"arn:aws:catalog:us-east-1:123456789012:portfolio/port-a1b2c3d4\"\n    },\n    \"DisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name to use for display purposes.\",\n      \"example\": \"My IT Portfolio\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description\
  \ of the portfolio.\",\n      \"example\": \"Approved IT services for the engineering team\"\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC time stamp of the creation time.\"\n    },\n    \"ProviderName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the portfolio provider.\",\n      \"example\": \"IT Team\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-service-catalog/refs/heads/main/json-schema/amazon-service-catalog-portfolio-schema.json
tags:
- AWS
- Cloud Governance
- Compliance
- IT Governance
- Service Catalog
title: Portfolio
---
