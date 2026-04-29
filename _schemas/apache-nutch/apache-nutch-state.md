---
description: The current state of a job.
layout: schema
name: State
properties_list: []
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-state-schema.json
slug: apache-nutch-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-state-schema.json\",\n  \"title\": \"State\",\n  \"description\": \"The current state of a job.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"IDLE\",\n    \"RUNNING\",\n    \"FINISHED\",\n    \"FAILED\",\n    \"KILLED\",\n    \"STOPPING\",\n    \"KILLING\",\n    \"ANY\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-state-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: State
---
