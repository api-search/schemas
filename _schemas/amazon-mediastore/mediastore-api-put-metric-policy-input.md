---
description: PutMetricPolicyInput schema from Amazon MediaStore API
layout: schema
name: PutMetricPolicyInput
properties_list:
- description: ''
  name: ContainerName
  type: object
- description: ''
  name: MetricPolicy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-put-metric-policy-input-schema.json
slug: mediastore-api-put-metric-policy-input
source_filename: mediastore-api-put-metric-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-metric-policy-input-schema.json\",\n  \"title\": \"PutMetricPolicyInput\",\n  \"description\": \"PutMetricPolicyInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container that you want to add the metric policy to.\"\n        }\n      ]\n    },\n    \"MetricPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricPolicy\"\n        },\n        {\n          \"description\": \"<p>The metric policy that you want to associate with the container. In the policy, you must indicate whether you want MediaStore to send container-level metrics.\
  \ You can also include up to five rules to define groups of objects that you want MediaStore to send object-level metrics for. If you include rules in the policy, construct each rule with both of the following:</p> <ul> <li> <p>An object group that defines which objects to include in the group. The definition can be a path or a file name, but it can't have more than 900 characters. Valid characters are: a-z, A-Z, 0-9, _ (underscore), = (equal), : (colon), . (period), - (hyphen), ~ (tilde), / (forward slash), and * (asterisk). Wildcards (*) are acceptable.</p> </li> <li> <p>An object group name that allows you to refer to the object group. The name can't have more than 30 characters. Valid characters are: a-z, A-Z, 0-9, and _ (underscore).</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\",\n    \"MetricPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-metric-policy-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PutMetricPolicyInput
---
