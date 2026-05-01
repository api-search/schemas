---
description: PutResourcePolicyRequest schema from Amazon X-Ray API
layout: schema
name: PutResourcePolicyRequest
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
  name: BypassPolicyLockoutCheck
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-put-resource-policy-request-schema.json
slug: xray-put-resource-policy-request
source_filename: xray-put-resource-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"PolicyName\",\n    \"PolicyDocument\"\n  ],\n  \"title\": \"PutResourcePolicyRequest\",\n  \"properties\": {\n    \"PolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyName\"\n        },\n        {\n          \"description\": \"The name of the resource policy. Must be unique within a specific Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"PolicyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"The resource policy document, which can be up to 5kb in size.\"\n        }\n      ]\n    },\n    \"PolicyRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevisionId\"\n        },\n        {\n          \"description\": \"<p>Specifies a specific policy revision, to ensure an atomic create operation. By default the resource\
  \ policy is created if it does not exist, or updated with an incremented revision id. The revision id is unique to each policy in the account.</p> <p>If the policy revision id does not match the latest revision id, the operation will fail with an <code>InvalidPolicyRevisionIdException</code> exception. You can also provide a <code>PolicyRevisionId</code> of 0. In this case, the operation will fail with an <code>InvalidPolicyRevisionIdException</code> exception if a resource policy with the same name already exists. </p>\"\n        }\n      ]\n    },\n    \"BypassPolicyLockoutCheck\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A flag to indicate whether to bypass the resource policy lockout safety check.</p> <important> <p>Setting this value to true increases the risk that the policy becomes unmanageable. Do not set this value to true indiscriminately.</p> </important> <p>Use this parameter\
  \ only when you include a policy in the request and you intend to prevent the principal that is making the request from making a subsequent <code>PutResourcePolicy</code> request.</p> <p>The default value is false.</p>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-resource-policy-request-schema.json\",\n  \"description\": \"PutResourcePolicyRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-resource-policy-request-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: PutResourcePolicyRequest
---
