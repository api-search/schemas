---
description: A render job in OpenCue
layout: schema
name: Job
properties_list:
- description: Unique job identifier
  name: id
  type: string
- description: Full job name
  name: name
  type: string
- description: Show name this job belongs to
  name: show
  type: string
- description: Current job state
  name: state
  type: string
- description: Job priority (higher is more important)
  name: priority
  type: integer
- description: Total number of frames in the job
  name: totalFrames
  type: integer
- description: Number of completed frames
  name: doneFrames
  type: integer
- description: Number of currently running frames
  name: runningFrames
  type: integer
- description: Number of failed/dead frames
  name: deadFrames
  type: integer
- description: Number of frames waiting to be dispatched
  name: waitingFrames
  type: integer
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
schema_file: json-schema/opencue-job-schema.json
slug: opencue-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"A render job in OpenCue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique job identifier\",\n      \"example\": \"job-def456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full job name\",\n      \"example\": \"feature_film_2026-shot_001-render_v001\"\n    },\n    \"show\": {\n      \"type\": \"string\",\n      \"description\": \"Show name this job belongs to\",\n      \"example\": \"feature_film_2026\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current job state\",\n      \"example\": \"RUNNING\",\n      \"enum\": [\n        \"PENDING\",\n        \"RUNNING\",\n        \"FINISHED\"\
  ,\n        \"PAUSED\"\n      ]\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Job priority (higher is more important)\",\n      \"example\": 100\n    },\n    \"totalFrames\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of frames in the job\",\n      \"example\": 100\n    },\n    \"doneFrames\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of completed frames\",\n      \"example\": 45\n    },\n    \"runningFrames\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently running frames\",\n      \"example\": 8\n    },\n    \"deadFrames\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of failed/dead frames\",\n      \"example\": 0\n    },\n    \"waitingFrames\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of frames waiting to be dispatched\",\n      \"example\": 47\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-job-schema.json
tags:
- Animation
- Color Management
- Film
- Linux Foundation
- Open Source
- Rendering
- Standards
- Visual Effects
- VFX
title: Job
---
