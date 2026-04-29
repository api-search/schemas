---
description: ReplicationSetArnList schema
layout: schema
name: ReplicationSetArnList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-replication-set-arn-list-schema.json
slug: incident-manager-replication-set-arn-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-replication-set-arn-list-schema.json\",\n  \"title\": \"ReplicationSetArnList\",\n  \"description\": \"ReplicationSetArnList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^arn:aws(-cn|-us-gov)?:[a-z0-9-]*:[a-z0-9-]*:([0-9]{12})?:.+$\",\n    \"minLength\": 0,\n    \"maxLength\": 1000\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-replication-set-arn-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ReplicationSetArnList
---
