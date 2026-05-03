---
description: A Run represents a single execution of a tenant's integration sync, tracking its status, mode, and timing information.
layout: schema
name: Pandium Run
properties_list:
- description: Unique identifier for the run.
  name: id
  type: integer
- description: ID of the tenant this run belongs to.
  name: tenant_id
  type: integer
- description: The trigger ID associated with this run.
  name: trigger_id
  type: string
- description: Current status of the run.
  name: status
  type: string
- description: The mode the run was triggered with.
  name: mode
  type: string
- description: Date and time the run was created.
  name: created_date
  type: string
- description: Date and time the run was last modified.
  name: modified_date
  type: string
- description: Date and time the run started executing.
  name: started_date
  type: string
- description: Date and time the run completed.
  name: completed_date
  type: string
provider_name: Pandium
provider_slug: pandium
schema_file: json-schema/run.json
slug: run
source_filename: run.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/pandium/blob/main/json-schema/run.json\",\n  \"title\": \"Pandium Run\",\n  \"description\": \"A Run represents a single execution of a tenant's integration sync, tracking its status, mode, and timing information.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"tenant_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the run.\"\n    },\n    \"tenant_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the tenant this run belongs to.\"\n    },\n    \"trigger_id\": {\n      \"type\": \"string\",\n      \"description\": \"The trigger ID associated with this run.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the run.\",\n      \"enum\": [\"pending\", \"running\", \"completed\", \"failed\"]\n    },\n    \"mode\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The mode the run was triggered with.\",\n      \"enum\": [\"cron\", \"manual\", \"webhook\", \"api\"]\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the run was created.\"\n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the run was last modified.\"\n    },\n    \"started_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the run started executing.\"\n    },\n    \"completed_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the run completed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/json-schema/run.json
tags:
- B2B
- Hubs
- Integrations
- Workflows
title: Pandium Run
---
