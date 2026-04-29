---
description: Schema for a job execution record in the Red Hat Ansible Automation Platform, representing a single run of a job template including its status, timing, and output metadata.
layout: schema
name: Red Hat Ansible Automation Platform Job
properties_list:
- description: The unique numeric identifier of the job execution.
  name: id
  type: integer
- description: The name of the job, typically inherited from the job template.
  name: name
  type: string
- description: A description of the job.
  name: description
  type: string
- description: The current execution status of the job.
  name: status
  type: string
- description: Whether the job execution resulted in a failure.
  name: failed
  type: boolean
- description: The ISO 8601 timestamp when job execution began.
  name: started
  type:
  - string
  - 'null'
- description: The ISO 8601 timestamp when job execution completed.
  name: finished
  type:
  - string
  - 'null'
- description: The elapsed wall-clock time in seconds for the job execution.
  name: elapsed
  type: number
- description: The type of job that was executed.
  name: job_type
  type: string
- description: How the job was launched.
  name: launch_type
  type: string
- description: The ID of the job template that was executed.
  name: job_template
  type: integer
- description: The ID of the inventory targeted by this job.
  name: inventory
  type: integer
- description: The ID of the project containing the playbook.
  name: project
  type: integer
- description: The playbook filename that was executed.
  name: playbook
  type: string
- description: The number of parallel processes used for execution.
  name: forks
  type: integer
- description: The host pattern used to limit the inventory scope.
  name: limit
  type: string
- description: The verbosity level of the job output (0=normal, 5=maximum debug).
  name: verbosity
  type: integer
- description: Extra variables passed to the playbook in YAML or JSON format.
  name: extra_vars
  type: string
- description: Artifacts collected during job execution, such as set_stats data.
  name: artifacts
  type: object
- description: Summary counts of host statuses from job execution.
  name: host_status_counts
  type: object
- description: The ISO 8601 timestamp when the job record was created.
  name: created
  type: string
- description: The ISO 8601 timestamp when the job record was last modified.
  name: modified
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-ansible-job-schema.json
slug: red-hat-ansible-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.redhat.com/schemas/red-hat/ansible-job.json\",\n  \"title\": \"Red Hat Ansible Automation Platform Job\",\n  \"description\": \"Schema for a job execution record in the Red Hat Ansible Automation Platform, representing a single run of a job template including its status, timing, and output metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique numeric identifier of the job execution.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job, typically inherited from the job template.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the job.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current execution status\
  \ of the job.\",\n      \"enum\": [\n        \"new\",\n        \"pending\",\n        \"waiting\",\n        \"running\",\n        \"successful\",\n        \"failed\",\n        \"error\",\n        \"canceled\"\n      ]\n    },\n    \"failed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job execution resulted in a failure.\",\n      \"default\": false\n    },\n    \"started\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when job execution began.\"\n    },\n    \"finished\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when job execution completed.\"\n    },\n    \"elapsed\": {\n      \"type\": \"number\",\n      \"description\": \"The elapsed wall-clock time in seconds for the job execution.\",\n      \"minimum\": 0\n    },\n    \"job_type\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ type of job that was executed.\",\n      \"enum\": [\"run\", \"check\"]\n    },\n    \"launch_type\": {\n      \"type\": \"string\",\n      \"description\": \"How the job was launched.\",\n      \"enum\": [\n        \"manual\",\n        \"relaunch\",\n        \"callback\",\n        \"scheduled\",\n        \"dependency\",\n        \"workflow\",\n        \"sync\",\n        \"scm\"\n      ]\n    },\n    \"job_template\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the job template that was executed.\"\n    },\n    \"inventory\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the inventory targeted by this job.\"\n    },\n    \"project\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project containing the playbook.\"\n    },\n    \"playbook\": {\n      \"type\": \"string\",\n      \"description\": \"The playbook filename that was executed.\"\n    },\n    \"forks\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"The number of parallel processes used for execution.\",\n      \"minimum\": 0\n    },\n    \"limit\": {\n      \"type\": \"string\",\n      \"description\": \"The host pattern used to limit the inventory scope.\"\n    },\n    \"verbosity\": {\n      \"type\": \"integer\",\n      \"description\": \"The verbosity level of the job output (0=normal, 5=maximum debug).\",\n      \"minimum\": 0,\n      \"maximum\": 5\n    },\n    \"extra_vars\": {\n      \"type\": \"string\",\n      \"description\": \"Extra variables passed to the playbook in YAML or JSON format.\"\n    },\n    \"artifacts\": {\n      \"type\": \"object\",\n      \"description\": \"Artifacts collected during job execution, such as set_stats data.\",\n      \"additionalProperties\": true\n    },\n    \"host_status_counts\": {\n      \"type\": \"object\",\n      \"description\": \"Summary counts of host statuses from job execution.\",\n      \"properties\": {\n        \"ok\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"Hosts that completed successfully with no changes.\"\n        },\n        \"changed\": {\n          \"type\": \"integer\",\n          \"description\": \"Hosts where changes were made.\"\n        },\n        \"failed\": {\n          \"type\": \"integer\",\n          \"description\": \"Hosts where execution failed.\"\n        },\n        \"skipped\": {\n          \"type\": \"integer\",\n          \"description\": \"Hosts that were skipped.\"\n        },\n        \"unreachable\": {\n          \"type\": \"integer\",\n          \"description\": \"Hosts that were unreachable.\"\n        },\n        \"dark\": {\n          \"type\": \"integer\",\n          \"description\": \"Hosts in dark state (unreachable).\"\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the job record was created.\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the job record was last modified.\"\n    }\n  },\n  \"$defs\": {\n    \"JobTemplate\": {\n      \"type\": \"object\",\n      \"description\": \"A job template defining the parameters for running an Ansible playbook.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the job template.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the job template.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the job template.\"\n        },\n        \"job_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"run\", \"check\"]\n        },\n        \"inventory\": {\n          \"type\": \"integer\"\n        },\n        \"project\": {\n          \"type\": \"integer\"\
  \n        },\n        \"playbook\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"id\": 4567,\n      \"name\": \"Deploy Web Application\",\n      \"status\": \"successful\",\n      \"failed\": false,\n      \"started\": \"2024-06-15T10:30:00Z\",\n      \"finished\": \"2024-06-15T10:35:42Z\",\n      \"elapsed\": 342.5,\n      \"job_type\": \"run\",\n      \"launch_type\": \"manual\",\n      \"job_template\": 123,\n      \"inventory\": 45,\n      \"project\": 67,\n      \"playbook\": \"deploy.yml\",\n      \"forks\": 5,\n      \"verbosity\": 0,\n      \"host_status_counts\": {\n        \"ok\": 8,\n        \"changed\": 5,\n        \"failed\": 0,\n        \"skipped\": 2,\n        \"unreachable\": 0\n      },\n      \"created\": \"2024-06-15T10:29:55Z\",\n      \"modified\": \"2024-06-15T10:35:42Z\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-ansible-job-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Red Hat Ansible Automation Platform Job
---
