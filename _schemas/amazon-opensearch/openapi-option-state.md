---
description: '<p>The state of a requested change. One of the following:</p> <ul> <li>Processing: The request change is still in-process.</li> <li>Active: The request change is processed and deployed to the Elasticsearch domain.</li> </ul>'
layout: schema
name: OptionState
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-option-state-schema.json
slug: openapi-option-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-option-state-schema.json\",\n  \"title\": \"OptionState\",\n  \"description\": \"<p>The state of a requested change. One of the following:</p> <ul> <li>Processing: The request change is still in-process.</li> <li>Active: The request change is processed and deployed to the Elasticsearch domain.</li> </ul>\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"RequiresIndexDocuments\",\n    \"Processing\",\n    \"Active\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-option-state-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: OptionState
---
