---
description: The broker's status.
layout: schema
name: BrokerState
properties_list: []
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-broker-state-schema.json
slug: mq-api-broker-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-state-schema.json\",\n  \"title\": \"BrokerState\",\n  \"description\": \"The broker's status.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CREATION_IN_PROGRESS\",\n    \"CREATION_FAILED\",\n    \"DELETION_IN_PROGRESS\",\n    \"RUNNING\",\n    \"REBOOT_IN_PROGRESS\",\n    \"CRITICAL_ACTION_REQUIRED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-state-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BrokerState
---
