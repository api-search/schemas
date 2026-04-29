---
description: Failover Condition settings. There can be multiple failover conditions inside AutomaticInputFailoverSettings.
layout: schema
name: FailoverCondition
properties_list:
- description: ''
  name: FailoverConditionSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-failover-condition-schema.json
slug: medialive-api-failover-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-failover-condition-schema.json\",\n  \"title\": \"FailoverCondition\",\n  \"description\": \"Failover Condition settings. There can be multiple failover conditions inside AutomaticInputFailoverSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailoverConditionSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailoverConditionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"failoverConditionSettings\"\n          },\n          \"description\": \"Failover condition type-specific settings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-failover-condition-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FailoverCondition
---
