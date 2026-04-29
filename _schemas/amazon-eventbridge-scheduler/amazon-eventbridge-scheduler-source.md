---
description: Source schema from Amazon EventBridge Scheduler
layout: schema
name: Source
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-source-schema.json
slug: amazon-eventbridge-scheduler-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-source-schema.json\",\n  \"title\": \"Source\",\n  \"description\": \"Source schema from Amazon EventBridge Scheduler\",\n  \"type\": \"string\",\n  \"pattern\": \"^(?=[/\\\\.\\\\-_A-Za-z0-9]+)((?!aws\\\\.).*)|(\\\\$(\\\\.[\\\\w_-]+(\\\\[(\\\\d+|\\\\*)\\\\])*)*)$\",\n  \"minLength\": 1,\n  \"maxLength\": 256\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-source-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: Source
---
