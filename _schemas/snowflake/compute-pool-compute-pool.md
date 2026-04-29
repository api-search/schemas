---
description: A Snowflake compute pool definition.
layout: schema
name: ComputePool
properties_list:
- description: Minimum number of nodes for the compute pool.
  name: min_nodes
  type: integer
- description: Maximum number of nodes for the compute pool.
  name: max_nodes
  type: integer
- description: Instance family for the compute pool.
  name: instance_family
  type: string
- description: Whether Snowflake automatically resumes the compute pool when any statement that requires the compute pool is submitted.
  name: auto_resume
  type: boolean
- description: Comment describing the compute pool.
  name: comment
  type: string
- description: Current state of the compute pool. Possible values include UNKNOWN, STARTING, IDLE, ACTIVE, STOPPING, SUSPENDED, and RESIZING.
  name: state
  type: string
- description: Number of services on the compute pool.
  name: num_services
  type: integer
- description: Number of jobs on the compute pool.
  name: num_jobs
  type: integer
- description: Number of seconds until the compute pool automatically suspends.
  name: auto_suspend_secs
  type: integer
- description: Number of currently active nodes on the compute pool.
  name: active_nodes
  type: integer
- description: Number of currently idle nodes on the compute pool.
  name: idle_nodes
  type: integer
- description: Number of target nodes on the compute pool.
  name: target_nodes
  type: integer
- description: Time the compute pool was created.
  name: created_on
  type: string
- description: Time the compute pool was last resumed.
  name: resumed_on
  type: string
- description: Time the compute pool was last updated.
  name: updated_on
  type: string
- description: Identifier for the current owner of the compute pool.
  name: owner
  type: string
- description: Whether a compute pool is created exclusively for a Snowflake Native App.
  name: is_exclusive
  type: boolean
- description: Name of the Snowflake Native App if the compute pool is created exclusively for the app.
  name: application
  type: string
- description: The name of the budget monitoring the credit usage of the compute pool.
  name: budget
  type: string
- description: Current error the compute pool hit if any.
  name: error_code
  type: string
- description: Current status of the compute pool if any.
  name: status_message
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/compute-pool-compute-pool-schema.json
slug: compute-pool-compute-pool
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComputePool\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake compute pool definition.\",\n  \"properties\": {\n    \"min_nodes\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of nodes for the compute pool.\"\n    },\n    \"max_nodes\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of nodes for the compute pool.\"\n    },\n    \"instance_family\": {\n      \"type\": \"string\",\n      \"description\": \"Instance family for the compute pool.\"\n    },\n    \"auto_resume\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Snowflake automatically resumes the compute pool when any statement that requires the compute pool is submitted.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment describing the compute pool.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Current state of the compute pool. Possible values include UNKNOWN, STARTING, IDLE, ACTIVE, STOPPING, SUSPENDED, and RESIZING.\"\n    },\n    \"num_services\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of services on the compute pool.\"\n    },\n    \"num_jobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of jobs on the compute pool.\"\n    },\n    \"auto_suspend_secs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seconds until the compute pool automatically suspends.\"\n    },\n    \"active_nodes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently active nodes on the compute pool.\"\n    },\n    \"idle_nodes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently idle nodes on the compute pool.\"\n    },\n    \"target_nodes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of target nodes on the compute pool.\"\n    },\n\
  \    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Time the compute pool was created.\"\n    },\n    \"resumed_on\": {\n      \"type\": \"string\",\n      \"description\": \"Time the compute pool was last resumed.\"\n    },\n    \"updated_on\": {\n      \"type\": \"string\",\n      \"description\": \"Time the compute pool was last updated.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the current owner of the compute pool.\"\n    },\n    \"is_exclusive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a compute pool is created exclusively for a Snowflake Native App.\"\n    },\n    \"application\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Snowflake Native App if the compute pool is created exclusively for the app.\"\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the budget monitoring the credit usage of the compute pool.\"\
  \n    },\n    \"error_code\": {\n      \"type\": \"string\",\n      \"description\": \"Current error the compute pool hit if any.\"\n    },\n    \"status_message\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the compute pool if any.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/compute-pool-compute-pool-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ComputePool
---
