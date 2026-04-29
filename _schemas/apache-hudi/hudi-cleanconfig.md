---
description: Hudi table cleaning configuration for managing old file versions
layout: schema
name: CleanConfig
properties_list:
- description: Cleaning policy (KEEP_LATEST_COMMITS or KEEP_LATEST_FILE_VERSIONS)
  name: policy
  type: string
- description: Number of commits to retain (for KEEP_LATEST_COMMITS)
  name: retainCommits
  type: integer
- description: Number of file versions to retain (for KEEP_LATEST_FILE_VERSIONS)
  name: retainFileVersions
  type: integer
- description: When to trigger cleaning (NUM_COMMITS or TIME_ELAPSED_SECONDS)
  name: triggerStrategy
  type: string
provider_name: Apache Hudi
provider_slug: apache-hudi
schema_file: json-schema/hudi-cleanconfig-schema.json
slug: hudi-cleanconfig
source_filename: hudi-cleanconfig-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hudi/json-schema/hudi-cleanconfig-schema.json\",\n  \"title\": \"CleanConfig\",\n  \"type\": \"object\",\n  \"description\": \"Hudi table cleaning configuration for managing old file versions\",\n  \"properties\": {\n    \"policy\": {\n      \"type\": \"string\",\n      \"description\": \"Cleaning policy (KEEP_LATEST_COMMITS or KEEP_LATEST_FILE_VERSIONS)\",\n      \"example\": \"KEEP_LATEST_COMMITS\"\n    },\n    \"retainCommits\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of commits to retain (for KEEP_LATEST_COMMITS)\",\n      \"example\": 10\n    },\n    \"retainFileVersions\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of file versions to retain (for KEEP_LATEST_FILE_VERSIONS)\",\n      \"example\": 3\n    },\n    \"triggerStrategy\": {\n      \"type\": \"string\",\n      \"description\": \"When to trigger cleaning\
  \ (NUM_COMMITS or TIME_ELAPSED_SECONDS)\",\n      \"example\": \"NUM_COMMITS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hudi/refs/heads/main/json-schema/hudi-cleanconfig-schema.json
tags:
- ACID
- Apache
- Big Data
- Data Lake
- Incremental Processing
- Lakehouse
- Open Source
title: CleanConfig
---
