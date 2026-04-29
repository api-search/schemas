---
description: List of limits that are specific to a given InstanceType and for each of it's <code> <a>InstanceRole</a> </code> .
layout: schema
name: AdditionalLimit
properties_list:
- description: ''
  name: LimitName
  type: object
- description: ''
  name: LimitValues
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-additional-limit-schema.json
slug: openapi-additional-limit
source_filename: openapi-additional-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-additional-limit-schema.json\",\n  \"title\": \"AdditionalLimit\",\n  \"description\": \" List of limits that are specific to a given InstanceType and for each of it's <code> <a>InstanceRole</a> </code> . \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LimitName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitName\"\n        },\n        {\n          \"description\": \" Name of Additional Limit is specific to a given InstanceType and for each of it's <code> <a>InstanceRole</a> </code> etc. <br/> Attributes and their details: <br/> <ul> <li>MaximumNumberOfDataNodesSupported</li> This attribute will be present in Master node only to specify how much data nodes upto which given <code> <a>ESPartitionInstanceType</a> </code> can support as master node.\
  \ <li>MaximumNumberOfDataNodesWithoutMasterNode</li> This attribute will be present in Data node only to specify how much data nodes of given <code> <a>ESPartitionInstanceType</a> </code> upto which you don't need any master nodes to govern them. </ul> \"\n        }\n      ]\n    },\n    \"LimitValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitValueList\"\n        },\n        {\n          \"description\": \" Value for given <code> <a>AdditionalLimit$LimitName</a> </code> . \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-additional-limit-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AdditionalLimit
---
