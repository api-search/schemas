---
description: Status of deployment process.
layout: schema
name: DeploymentStatus
properties_list: []
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-deployment-status-schema.json
slug: rest-api-deployment-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-deployment-status-schema.json\",\n  \"title\": \"DeploymentStatus\",\n  \"description\": \"Status of deployment process.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"UPLOADING\",\n    \"DEPLOYED\",\n    \"OBSOLETE\",\n    \"REMOVING\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-deployment-status-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: DeploymentStatus
---
