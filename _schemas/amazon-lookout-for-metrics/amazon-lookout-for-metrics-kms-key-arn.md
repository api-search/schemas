---
description: KmsKeyArn schema from Amazon Lookout for Metrics API
layout: schema
name: KmsKeyArn
properties_list: []
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-kms-key-arn-schema.json
slug: amazon-lookout-for-metrics-kms-key-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-kms-key-arn-schema.json\",\n  \"title\": \"KmsKeyArn\",\n  \"description\": \"KmsKeyArn schema from Amazon Lookout for Metrics API\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws.*:kms:.*:[0-9]{12}:key/[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}\",\n  \"minLength\": 20,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-kms-key-arn-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: KmsKeyArn
---
