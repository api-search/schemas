---
description: Current state of an experiment
layout: schema
name: ExperimentState
properties_list:
- description: Experiment status
  name: status
  type: string
- description: Status reason
  name: reason
  type: string
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-experiment-state-schema.json
slug: amazon-fis-experiment-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-state-schema.json\",\n  \"title\": \"ExperimentState\",\n  \"description\": \"Current state of an experiment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Experiment status\",\n      \"example\": \"running\",\n      \"enum\": [\n        \"pending\",\n        \"initiating\",\n        \"running\",\n        \"completed\",\n        \"stopping\",\n        \"stopped\",\n        \"failed\"\n      ]\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Status reason\",\n      \"example\": \"Experiment running normally\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-state-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: ExperimentState
---
