---
description: A job template defines the parameters for running an Ansible playbook against an inventory of managed hosts.
layout: schema
name: JobTemplate
properties_list:
- description: The unique identifier of the job template.
  name: id
  type: integer
- description: The name of the job template.
  name: name
  type: string
- description: A description of the job template.
  name: description
  type: string
- description: The type of job to execute.
  name: job_type
  type: string
- description: The ID of the inventory to run against.
  name: inventory
  type: integer
- description: The ID of the project containing the playbook.
  name: project
  type: integer
- description: The playbook filename to execute from the project.
  name: playbook
  type: string
- description: The number of parallel processes to use for execution.
  name: forks
  type: integer
- description: A host pattern to further limit the inventory scope.
  name: limit
  type: string
- description: The verbosity level for job output (0-5).
  name: verbosity
  type: integer
- description: Extra variables in YAML or JSON format.
  name: extra_vars
  type: string
- description: Whether to prompt for extra variables on launch.
  name: ask_variables_on_launch
  type: boolean
- description: Whether to prompt for inventory on launch.
  name: ask_inventory_on_launch
  type: boolean
- description: Whether to prompt for credentials on launch.
  name: ask_credential_on_launch
  type: boolean
- description: Whether the survey is enabled for this template.
  name: survey_enabled
  type: boolean
- description: The date and time the template was created.
  name: created
  type: string
- description: The date and time the template was last modified.
  name: modified
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-ansible-automation-platform-job-template-schema.json
slug: red-hat-ansible-automation-platform-job-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobTemplate\",\n  \"type\": \"object\",\n  \"description\": \"A job template defines the parameters for running an Ansible playbook against an inventory of managed hosts.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the job template.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job template.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the job template.\"\n    },\n    \"job_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of job to execute.\"\n    },\n    \"inventory\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the inventory to run against.\"\n    },\n    \"project\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project containing\
  \ the playbook.\"\n    },\n    \"playbook\": {\n      \"type\": \"string\",\n      \"description\": \"The playbook filename to execute from the project.\"\n    },\n    \"forks\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of parallel processes to use for execution.\"\n    },\n    \"limit\": {\n      \"type\": \"string\",\n      \"description\": \"A host pattern to further limit the inventory scope.\"\n    },\n    \"verbosity\": {\n      \"type\": \"integer\",\n      \"description\": \"The verbosity level for job output (0-5).\"\n    },\n    \"extra_vars\": {\n      \"type\": \"string\",\n      \"description\": \"Extra variables in YAML or JSON format.\"\n    },\n    \"ask_variables_on_launch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to prompt for extra variables on launch.\"\n    },\n    \"ask_inventory_on_launch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to prompt for inventory on launch.\"\n    },\n    \"\
  ask_credential_on_launch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to prompt for credentials on launch.\"\n    },\n    \"survey_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the survey is enabled for this template.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the template was created.\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the template was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-ansible-automation-platform-job-template-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: JobTemplate
---
