---
description: Paginated collection of targets.
layout: schema
name: TargetCollection
properties_list:
- description: ''
  name: items
  type: array
- description: Total number of targets matching the query.
  name: totalCount
  type: integer
- description: Maximum items per page.
  name: limit
  type: integer
- description: Current offset in the result set.
  name: offset
  type: integer
- description: Whether more results are available.
  name: hasMore
  type: boolean
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-target-collection-schema.json
slug: oracle-enterprise-manager-cloud-control-target-collection
source_filename: oracle-enterprise-manager-cloud-control-target-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TargetCollection\",\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of targets.\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of targets matching the query.\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum items per page.\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Current offset in the result set.\"\n    },\n    \"hasMore\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether more results are available.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-target-collection-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: TargetCollection
---
