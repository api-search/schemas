---
description: 'The status of a classification job. Possible values are:'
layout: schema
name: JobStatus
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-job-status-schema.json
slug: amazon-macie-job-status
source_filename: amazon-macie-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"The status of a classification job. Possible values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"RUNNING\",\n    \"PAUSED\",\n    \"CANCELLED\",\n    \"COMPLETE\",\n    \"IDLE\",\n    \"USER_PAUSED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-status-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: JobStatus
---
