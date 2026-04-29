---
description: Paginated collection of incidents.
layout: schema
name: IncidentCollection
properties_list:
- description: ''
  name: items
  type: array
- description: Total number of incidents matching the query.
  name: totalCount
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: hasMore
  type: boolean
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-incident-collection-schema.json
slug: oracle-enterprise-manager-cloud-control-incident-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentCollection\",\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of incidents.\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of incidents matching the query.\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"hasMore\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-incident-collection-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: IncidentCollection
---
