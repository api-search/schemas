---
description: ListClustersResult schema from Amazon Snow Family API
layout: schema
name: ListClustersResult
properties_list:
- description: ''
  name: ClusterListEntries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-clusters-result-schema.json
slug: amazon-snow-family-list-clusters-result
source_filename: amazon-snow-family-list-clusters-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-clusters-result-schema.json\",\n  \"title\": \"ListClustersResult\",\n  \"description\": \"ListClustersResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterListEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterListEntryList\"\n        },\n        {\n          \"description\": \"Each <code>ClusterListEntry</code> object contains a cluster's state, a cluster's ID, and other important status information.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP requests are stateless. If you use the automatically generated <code>NextToken</code> value\
  \ in your next <code>ClusterListEntry</code> call, your list of returned clusters will start from this point in the array.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-clusters-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListClustersResult
---
