---
description: The broker's deployment mode.
layout: schema
name: DeploymentMode
properties_list: []
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-deployment-mode-schema.json
slug: mq-api-deployment-mode
source_filename: mq-api-deployment-mode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-deployment-mode-schema.json\",\n  \"title\": \"DeploymentMode\",\n  \"description\": \"The broker's deployment mode.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SINGLE_INSTANCE\",\n    \"ACTIVE_STANDBY_MULTI_AZ\",\n    \"CLUSTER_MULTI_AZ\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-deployment-mode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DeploymentMode
---
