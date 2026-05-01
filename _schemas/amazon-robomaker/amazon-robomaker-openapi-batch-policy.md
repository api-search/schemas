---
description: Information about the batch policy.
layout: schema
name: BatchPolicy
properties_list:
- description: ''
  name: timeoutInSeconds
  type: object
- description: ''
  name: maxConcurrency
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-batch-policy-schema.json
slug: amazon-robomaker-openapi-batch-policy
source_filename: amazon-robomaker-openapi-batch-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-policy-schema.json\",\n  \"title\": \"BatchPolicy\",\n  \"description\": \"Information about the batch policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchTimeoutInSeconds\"\n        },\n        {\n          \"description\": \"<p>The amount of time, in seconds, to wait for the batch to complete. </p> <p>If a batch times out, and there are pending requests that were failing due to an internal failure (like <code>InternalServiceError</code>), they will be moved to the failed list and the batch status will be <code>Failed</code>. If the pending requests were failing for any other reason, the failed pending requests will be moved to the failed list and the batch\
  \ status will be <code>TimedOut</code>. </p>\"\n        }\n      ]\n    },\n    \"maxConcurrency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxConcurrency\"\n        },\n        {\n          \"description\": \"<p>The number of active simulation jobs create as part of the batch that can be in an active state at the same time. </p> <p>Active states include: <code>Pending</code>,<code>Preparing</code>, <code>Running</code>, <code>Restarting</code>, <code>RunningFailed</code> and <code>Terminating</code>. All other states are terminal states. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-policy-schema.json
tags:
- Robotics
- Simulation
title: BatchPolicy
---
