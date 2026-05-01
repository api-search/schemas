---
description: An object that contains two attributes, <code>SortBy</code> and <code>SortOrder</code>.
layout: schema
name: Sort
properties_list:
- description: ''
  name: SortBy
  type: object
- description: ''
  name: SortOrder
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-sort-schema.json
slug: amazon-marketplace-sort
source_filename: amazon-marketplace-sort-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-sort-schema.json\",\n  \"title\": \"Sort\",\n  \"description\": \"An object that contains two attributes, <code>SortBy</code> and <code>SortOrder</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortBy\"\n        },\n        {\n          \"description\": \"<p>For <code>ListEntities</code>, supported attributes include <code>LastModifiedDate</code> (default), <code>Visibility</code>, <code>EntityId</code>, and <code>Name</code>.</p> <p>For <code>ListChangeSets</code>, supported attributes include <code>StartTime</code> and <code>EndTime</code>.</p>\"\n        }\n      ]\n    },\n    \"SortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\
  \n        },\n        {\n          \"description\": \"The sorting order. Can be <code>ASCENDING</code> or <code>DESCENDING</code>. The default value is <code>DESCENDING</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-sort-schema.json
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
title: Sort
---
