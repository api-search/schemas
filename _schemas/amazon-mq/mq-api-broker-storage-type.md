---
description: <p>The broker's storage type.</p> <important><p>EFS is not supported for RabbitMQ engine type.</p></important>
layout: schema
name: BrokerStorageType
properties_list: []
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-broker-storage-type-schema.json
slug: mq-api-broker-storage-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-storage-type-schema.json\",\n  \"title\": \"BrokerStorageType\",\n  \"description\": \"<p>The broker's storage type.</p> <important><p>EFS is not supported for RabbitMQ engine type.</p></important>\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"EBS\",\n    \"EFS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-storage-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BrokerStorageType
---
