---
description: OpenSearch/Elasticsearch data source configuration
layout: schema
name: ElasticsearchDataSourceConfig
properties_list:
- description: OpenSearch endpoint URL
  name: endpoint
  type: string
- description: AWS Region
  name: awsRegion
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-elasticsearch-data-source-config-schema.json
slug: appsync-elasticsearch-data-source-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-elasticsearch-data-source-config-schema.json\",\n  \"title\": \"ElasticsearchDataSourceConfig\",\n  \"description\": \"OpenSearch/Elasticsearch data source configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"OpenSearch endpoint URL\"\n    },\n    \"awsRegion\": {\n      \"type\": \"string\",\n      \"description\": \"AWS Region\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-elasticsearch-data-source-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: ElasticsearchDataSourceConfig
---
