---
description: LogGroupArn schema from Amazon Managed Service for Prometheus API
layout: schema
name: LogGroupArn
properties_list: []
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-log-group-arn-schema.json
slug: amazon-managed-prometheus-log-group-arn
source_filename: amazon-managed-prometheus-log-group-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-log-group-arn-schema.json\",\n  \"title\": \"LogGroupArn\",\n  \"description\": \"LogGroupArn schema from Amazon Managed Service for Prometheus API\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws[a-z0-9-]*:logs:[a-z0-9-]+:\\\\d{12}:log-group:[A-Za-z0-9\\\\.\\\\-\\\\_\\\\#/]{1,512}\\\\:\\\\*\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-log-group-arn-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: LogGroupArn
---
