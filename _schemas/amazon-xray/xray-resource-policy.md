---
description: A resource policy grants one or more Amazon Web Services services and accounts permissions to access X-Ray. Each resource policy is associated with a specific Amazon Web Services account.
layout: schema
name: ResourcePolicy
properties_list:
- description: ''
  name: PolicyName
  type: object
- description: ''
  name: PolicyDocument
  type: object
- description: ''
  name: PolicyRevisionId
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-resource-policy-schema.json
slug: xray-resource-policy
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyName\"\n        },\n        {\n          \"description\": \"The name of the resource policy. Must be unique within a specific Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"PolicyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"The resource policy document, which can be up to 5kb in size.\"\n        }\n      ]\n    },\n    \"PolicyRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevisionId\"\n        },\n        {\n          \"description\": \"Returns the current policy revision id for this policy name.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n   \
  \     },\n        {\n          \"description\": \"When the policy was last updated, in Unix time seconds.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A resource policy grants one or more Amazon Web Services services and accounts permissions to access X-Ray. Each resource policy is associated with a specific Amazon Web Services account.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourcePolicy\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-resource-policy-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-resource-policy-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ResourcePolicy
---
