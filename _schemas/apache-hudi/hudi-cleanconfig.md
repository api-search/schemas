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
