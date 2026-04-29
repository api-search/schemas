---
description: Provides information for filtering a list of event detection jobs.
layout: schema
name: EventsDetectionJobFilter
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: SubmitTimeBefore
  type: object
- description: ''
  name: SubmitTimeAfter
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-events-detection-job-filter-schema.json
slug: openapi.yml-events-detection-job-filter
source_filename: openapi.yml-events-detection-job-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-events-detection-job-filter-schema.json\",\n  \"title\": \"EventsDetectionJobFilter\",\n  \"description\": \"Provides information for filtering a list of event detection jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"Filters on the name of the events detection job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"Filters the list of jobs based on job status. Returns only jobs with the specified status.\"\n        }\n      ]\n    },\n    \"SubmitTimeBefore\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filters the list of jobs based on the time that the job was submitted for processing. Returns only jobs submitted before the specified time. Jobs are returned in ascending order, oldest to newest.\"\n        }\n      ]\n    },\n    \"SubmitTimeAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filters the list of jobs based on the time that the job was submitted for processing. Returns only jobs submitted after the specified time. Jobs are returned in descending order, newest to oldest.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-events-detection-job-filter-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EventsDetectionJobFilter
---
