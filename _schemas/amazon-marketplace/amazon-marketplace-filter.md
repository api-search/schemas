---
description: A filter object, used to optionally filter results from calls to the <code>ListEntities</code> and <code>ListChangeSets</code> actions.
layout: schema
name: Filter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: ValueList
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-filter-schema.json
slug: amazon-marketplace-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"A filter object, used to optionally filter results from calls to the <code>ListEntities</code> and <code>ListChangeSets</code> actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterName\"\n        },\n        {\n          \"description\": \"<p>For <code>ListEntities</code>, the supported value for this is an <code>EntityId</code>.</p> <p>For <code>ListChangeSets</code>, the supported values are as follows:</p>\"\n        }\n      ]\n    },\n    \"ValueList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueList\"\n        },\n        {\n          \"description\": \"<p> <code>ListEntities</code>\
  \ - This is a list of unique <code>EntityId</code>s.</p> <p> <code>ListChangeSets</code> - The supported filter names and associated <code>ValueList</code>s is as follows:</p> <ul> <li> <p> <code>ChangeSetName</code> - The supported <code>ValueList</code> is a list of non-unique <code>ChangeSetName</code>s. These are defined when you call the <code>StartChangeSet</code> action.</p> </li> <li> <p> <code>Status</code> - The supported <code>ValueList</code> is a list of statuses for all change set requests.</p> </li> <li> <p> <code>EntityId</code> - The supported <code>ValueList</code> is a list of unique <code>EntityId</code>s.</p> </li> <li> <p> <code>BeforeStartTime</code> - The supported <code>ValueList</code> is a list of all change sets that started before the filter value.</p> </li> <li> <p> <code>AfterStartTime</code> - The supported <code>ValueList</code> is a list of all change sets that started after the filter value.</p> </li> <li> <p> <code>BeforeEndTime</code> - The supported\
  \ <code>ValueList</code> is a list of all change sets that ended before the filter value.</p> </li> <li> <p> <code>AfterEndTime</code> - The supported <code>ValueList</code> is a list of all change sets that ended after the filter value.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-filter-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: Filter
---
