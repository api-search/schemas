---
description: A Neon project is the top-level object in the Neon hierarchy containing branches, databases, roles, and compute endpoints for a serverless Postgres deployment.
layout: schema
name: Neon Project
properties_list:
- description: The unique project identifier assigned by Neon
  name: id
  type: string
- description: The cloud platform identifier
  name: platform_id
  type: string
- description: The cloud region where the project is deployed (e.g., aws-us-east-1, aws-eu-central-1)
  name: region_id
  type: string
- description: The human-readable project name
  name: name
  type: string
- description: The provisioner type used for compute resources
  name: provisioner
  type: string
- description: ''
  name: default_endpoint_settings
  type: object
- description: The Postgres major version number
  name: pg_version
  type: integer
- description: Whether connection passwords are stored and retrievable
  name: store_passwords
  type: boolean
- description: Total active time of compute endpoints in seconds
  name: active_time
  type: integer
- description: Total CPU seconds consumed by compute endpoints
  name: cpu_used_sec
  type: integer
- description: Scheduled maintenance window start time
  name: maintenance_starts_at
  type: string
- description: The source that created this project (e.g., console, api)
  name: creation_source
  type: string
- description: The organization ID this project belongs to
  name: org_id
  type: string
- description: Timestamp when the project was created
  name: created_at
  type: string
- description: Timestamp when the project was last updated
  name: updated_at
  type: string
provider_name: Neon
provider_slug: neon
schema_file: json-schema/neon-project-schema.json
slug: neon-project
source_filename: neon-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://neon.com/schemas/neon/project.json\",\n  \"title\": \"Neon Project\",\n  \"description\": \"A Neon project is the top-level object in the Neon hierarchy containing branches, databases, roles, and compute endpoints for a serverless Postgres deployment.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"region_id\", \"pg_version\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique project identifier assigned by Neon\"\n    },\n    \"platform_id\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud platform identifier\"\n    },\n    \"region_id\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud region where the project is deployed (e.g., aws-us-east-1, aws-eu-central-1)\",\n      \"enum\": [\n        \"aws-us-east-1\",\n        \"aws-us-east-2\",\n        \"aws-us-west-2\",\n        \"aws-eu-central-1\"\
  ,\n        \"aws-ap-southeast-1\",\n        \"aws-ap-southeast-2\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable project name\",\n      \"maxLength\": 64\n    },\n    \"provisioner\": {\n      \"type\": \"string\",\n      \"description\": \"The provisioner type used for compute resources\",\n      \"enum\": [\"k8s-pod\", \"k8s-neonvm\"]\n    },\n    \"default_endpoint_settings\": {\n      \"$ref\": \"#/$defs/EndpointSettings\"\n    },\n    \"pg_version\": {\n      \"type\": \"integer\",\n      \"description\": \"The Postgres major version number\",\n      \"enum\": [14, 15, 16, 17]\n    },\n    \"store_passwords\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether connection passwords are stored and retrievable\"\n    },\n    \"active_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Total active time of compute endpoints in seconds\",\n      \"minimum\": 0\n    },\n    \"cpu_used_sec\": {\n \
  \     \"type\": \"integer\",\n      \"description\": \"Total CPU seconds consumed by compute endpoints\",\n      \"minimum\": 0\n    },\n    \"maintenance_starts_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled maintenance window start time\"\n    },\n    \"creation_source\": {\n      \"type\": \"string\",\n      \"description\": \"The source that created this project (e.g., console, api)\"\n    },\n    \"org_id\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID this project belongs to\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was last updated\"\n    }\n  },\n  \"$defs\": {\n    \"EndpointSettings\": {\n      \"type\": \"object\",\n    \
  \  \"description\": \"Default settings applied to new compute endpoints in this project\",\n      \"properties\": {\n        \"autoscaling_limit_min_cu\": {\n          \"type\": \"number\",\n          \"description\": \"Minimum compute units for autoscaling\",\n          \"minimum\": 0.25\n        },\n        \"autoscaling_limit_max_cu\": {\n          \"type\": \"number\",\n          \"description\": \"Maximum compute units for autoscaling\",\n          \"minimum\": 0.25\n        },\n        \"suspend_timeout_seconds\": {\n          \"type\": \"integer\",\n          \"description\": \"Seconds of inactivity before the endpoint is automatically suspended\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/json-schema/neon-project-schema.json
tags:
- Databases
- Serverless
- Postgres
- Infrastructure
- Authentication
- Edge
title: Neon Project
---
