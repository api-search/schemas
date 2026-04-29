---
description: 'Type of Log File, it can be one of the following: <ul> <li>INDEX_SLOW_LOGS: Index slow logs contain insert requests that took more time than configured index query log threshold to execute.</li> <li>SEARCH_SLOW_LOGS: Search slow logs contain search queries that took more time than configured search query log threshold to execute.</li> <li>ES_APPLICATION_LOGS: Elasticsearch application logs contain information about errors and warnings raised during the operation of the service and can be useful for troubleshooting.</li> <li>AUDIT_LOGS: Audit logs contain records of user requests for access from the domain.</li> </ul>'
layout: schema
name: LogType
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-log-type-schema.json
slug: openapi-log-type
source_filename: openapi-log-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-log-type-schema.json\",\n  \"title\": \"LogType\",\n  \"description\": \"Type of Log File, it can be one of the following: <ul> <li>INDEX_SLOW_LOGS: Index slow logs contain insert requests that took more time than configured index query log threshold to execute.</li> <li>SEARCH_SLOW_LOGS: Search slow logs contain search queries that took more time than configured search query log threshold to execute.</li> <li>ES_APPLICATION_LOGS: Elasticsearch application logs contain information about errors and warnings raised during the operation of the service and can be useful for troubleshooting.</li> <li>AUDIT_LOGS: Audit logs contain records of user requests for access from the domain.</li> </ul> \",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INDEX_SLOW_LOGS\",\n    \"SEARCH_SLOW_LOGS\",\n    \"\
  ES_APPLICATION_LOGS\",\n    \"AUDIT_LOGS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-log-type-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: LogType
---
