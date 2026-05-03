---
description: A security filter in Oracle Essbase that controls member-level data access for a database. Filters define read, write, none, or metadata-read access for specific member combinations, enabling fine-grained security beyond application and database-level roles.
layout: schema
name: Oracle Essbase Filter
properties_list:
- description: Filter name used to reference this filter when assigning it to users or groups.
  name: name
  type: string
- description: Human-readable description of what the filter controls.
  name: description
  type: string
- description: Filter row definitions specifying the access level for each member combination.
  name: rows
  type: array
- description: HATEOAS navigation links.
  name: links
  type: array
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-filter-schema.json
slug: oracle-essbase-filter
source_filename: oracle-essbase-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-filter-schema.json\",\n  \"title\": \"Oracle Essbase Filter\",\n  \"description\": \"A security filter in Oracle Essbase that controls member-level data access for a database. Filters define read, write, none, or metadata-read access for specific member combinations, enabling fine-grained security beyond application and database-level roles.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Filter name used to reference this filter when assigning it to users or groups.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what the filter controls.\"\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"Filter row definitions specifying the access level for each member combination.\",\n      \"items\": {\n        \"$ref\"\
  : \"#/$defs/FilterRow\"\n      }\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"FilterRow\": {\n      \"type\": \"object\",\n      \"description\": \"A single row in a security filter defining the access level for a specific member or member combination.\",\n      \"properties\": {\n        \"access\": {\n          \"type\": \"string\",\n          \"description\": \"Access level granted for the specified member combination. READ allows data retrieval. WRITE allows data updates. NONE denies all access. METAREAD allows viewing member names but not data values.\",\n          \"enum\": [\"READ\", \"WRITE\", \"NONE\", \"METAREAD\"]\n        },\n        \"member\": {\n          \"type\": \"string\",\n          \"description\": \"Member specification or cross-dimensional member combination that this filter\
  \ row applies to.\"\n        }\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation link.\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link URL.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for this link.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Media type of the linked resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-filter-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Filter
---
