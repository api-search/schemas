---
description: SearchTablesRequest schema from Amazon Glue API
layout: schema
name: SearchTablesRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: SearchText
  type: object
- description: ''
  name: SortCriteria
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: ResourceShareType
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-search-tables-request-schema.json
slug: glue-search-tables-request
source_filename: glue-search-tables-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-search-tables-request-schema.json\",\n  \"title\": \"SearchTablesRequest\",\n  \"description\": \"SearchTablesRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"A unique identifier, consisting of <code> <i>account_id</i> </code>.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, included if this is a continuation call.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchPropertyPredicates\"\
  \n        },\n        {\n          \"description\": \"<p>A list of key-value pairs, and a comparator used to filter the search results. Returns all entities matching the predicate.</p> <p>The <code>Comparator</code> member of the <code>PropertyPredicate</code> struct is used only for time fields, and can be omitted for other field types. Also, when comparing string values, such as when <code>Key=Name</code>, a fuzzy match algorithm is used. The <code>Key</code> field (for example, the value of the <code>Name</code> field) is split on certain punctuation characters, for example, -, :, #, etc. into tokens. Then each token is exact-match compared with the <code>Value</code> member of <code>PropertyPredicate</code>. For example, if <code>Key=Name</code> and <code>Value=link</code>, tables named <code>customer-link</code> and <code>xx-link-yy</code> are returned, but <code>xxlinkyy</code> is not returned.</p>\"\n        }\n      ]\n    },\n    \"SearchText\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/ValueString\"\n        },\n        {\n          \"description\": \"<p>A string used for a text search.</p> <p>Specifying a value in quotes filters based on an exact match to the value.</p>\"\n        }\n      ]\n    },\n    \"SortCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortCriteria\"\n        },\n        {\n          \"description\": \"A list of criteria for sorting the results by a field name, in an ascending or descending order.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of tables to return in a single response.\"\n        }\n      ]\n    },\n    \"ResourceShareType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceShareType\"\n        },\n        {\n          \"description\": \"<p>Allows\
  \ you to specify that you want to search the tables shared with your account. The allowable values are <code>FOREIGN</code> or <code>ALL</code>. </p> <ul> <li> <p>If set to <code>FOREIGN</code>, will search the tables shared with your account. </p> </li> <li> <p>If set to <code>ALL</code>, will search the tables shared with your account, as well as the tables in yor local account. </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-search-tables-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: SearchTablesRequest
---
