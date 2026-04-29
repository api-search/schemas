---
description: CancelClusterRequest schema from Amazon Snow Family API
layout: schema
name: CancelClusterRequest
properties_list:
- description: ''
  name: ClusterId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-cancel-cluster-request-schema.json
slug: amazon-snow-family-cancel-cluster-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cancel-cluster-request-schema.json\",\n  \"title\": \"CancelClusterRequest\",\n  \"description\": \"CancelClusterRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterId\"\n        },\n        {\n          \"description\": \"The 39-character ID for the cluster that you want to cancel, for example <code>CID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClusterId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cancel-cluster-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CancelClusterRequest
---
