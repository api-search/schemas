---
description: Each <code>JobListEntry</code> object contains a job's state, a job's ID, and a value that indicates whether the job is a job part, in the case of an export job.
layout: schema
name: JobListEntry
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobState
  type: object
- description: ''
  name: IsMaster
  type: object
- description: ''
  name: JobType
  type: object
- description: ''
  name: SnowballType
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-job-list-entry-schema.json
slug: amazon-snow-family-job-list-entry
source_filename: amazon-snow-family-job-list-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-list-entry-schema.json\",\n  \"title\": \"JobListEntry\",\n  \"description\": \"Each <code>JobListEntry</code> object contains a job's state, a job's ID, and a value that indicates whether the job is a job part, in the case of an export job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a job, for example <code>JID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"JobState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobState\"\n        },\n        {\n          \"description\": \"The current state of this job.\"\n        }\n\
  \      ]\n    },\n    \"IsMaster\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A value that indicates that this job is a main job. A main job represents a successful request to create an export job. Main jobs aren't associated with any Snowballs. Instead, each main job will have at least one job part, and each job part is associated with a Snowball. It might take some time before the job parts associated with a particular main job are listed, because they are created after the main job is created.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"The type of job.\"\n        }\n      ]\n    },\n    \"SnowballType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballType\"\n        },\n        {\n          \"description\"\
  : \"The type of device used with this job.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date for this job.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The optional description of this specific job, for example <code>Important Photos 2016-08-11</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-list-entry-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: JobListEntry
---
