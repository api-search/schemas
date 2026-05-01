---
description: '<p>Specifies which metrics are gathered for the MSK cluster. This property has the following possible values: DEFAULT, PER_BROKER, PER_TOPIC_PER_BROKER, and PER_TOPIC_PER_PARTITION. For a list of the metrics associated with each of these levels of monitoring, see <a href="https://docs.aws.amazon.com/msk/latest/developerguide/monitoring.html">Monitoring</a>.</p>'
layout: schema
name: EnhancedMonitoring
properties_list: []
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-enhanced-monitoring-schema.json
slug: msk-api-enhanced-monitoring
source_filename: msk-api-enhanced-monitoring-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-enhanced-monitoring-schema.json\",\n  \"title\": \"EnhancedMonitoring\",\n  \"description\": \"\\n            <p>Specifies which metrics are gathered for the MSK cluster. This property has the following possible values: DEFAULT, PER_BROKER, PER_TOPIC_PER_BROKER, and PER_TOPIC_PER_PARTITION. For a list of the metrics associated with each of these levels of monitoring, see <a href=\\\"https://docs.aws.amazon.com/msk/latest/developerguide/monitoring.html\\\">Monitoring</a>.</p>\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DEFAULT\",\n    \"PER_BROKER\",\n    \"PER_TOPIC_PER_BROKER\",\n    \"PER_TOPIC_PER_PARTITION\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-enhanced-monitoring-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EnhancedMonitoring
---
