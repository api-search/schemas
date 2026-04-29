---
description: A Snowflake notebook
layout: schema
name: Notebook
properties_list:
- description: Name of the notebook
  name: name
  type: string
- description: User specified version alias
  name: version
  type: string
- description: Location to copy the file from. This must be a Snowflake stage location.
  name: fromLocation
  type: string
- description: Name + path of the file for the Notebook
  name: main_file
  type: string
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
- description: The default version name of a file based entity.
  name: default_version
  type: string
- description: Warehouse against which the queries issued by the Streamlit app are run against
  name: query_warehouse
  type: string
- description: Date and time when the notebook was created.
  name: created_on
  type: string
- description: Database in which the notebook is stored
  name: database_name
  type: string
- description: Schema in which the notebook is stored
  name: schema_name
  type: string
- description: Role that owns the notebook
  name: owner
  type: string
- description: The type of role that owns the notebook
  name: owner_role_type
  type: string
- description: Unique ID associated with the notebook object.
  name: url_id
  type: string
- description: User facing title of the Streamlit app or an Organization Profile
  name: title
  type: string
- description: Default packages of the notebook
  name: default_packages
  type: string
- description: User packages of the notebook
  name: user_packages
  type: string
- description: The runtime to run the Streamlit or Notebook on. If this is not set, the warehouse is assumed
  name: runtime_name
  type: string
- description: Compute pool name where the snowservice runs
  name: compute_pool
  type: string
- description: List of urls
  name: import_urls
  type: array
- description: List of external access integrations attached to this function
  name: external_access_integrations
  type: array
- description: Secrets to be used with this function for external access
  name: external_access_secrets
  type: string
- description: Sets the time in seconds for when to shutdown an idle Notebook.
  name: idle_auto_shutdown_time_seconds
  type: integer
- description: The current version location
  name: live_version_location_uri
  type: string
- description: Name of the budget if the notebook is monitored by a budget
  name: budget
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notebook-notebook-schema.json
slug: notebook-notebook
source_filename: notebook-notebook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Notebook\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake notebook\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the notebook\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"User specified version alias\"\n    },\n    \"fromLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Location to copy the file from. This must be a Snowflake stage location.\"\n    },\n    \"main_file\": {\n      \"type\": \"string\",\n      \"description\": \"Name + path of the file for the Notebook\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    },\n    \"default_version\": {\n      \"type\": \"string\",\n      \"description\": \"The default version name of a file based entity.\"\n    },\n    \"query_warehouse\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Warehouse against which the queries issued by the Streamlit app are run against\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the notebook was created.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the notebook is stored\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the notebook is stored\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the notebook\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the notebook\"\n    },\n    \"url_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID associated with the notebook object.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"User facing\
  \ title of the Streamlit app or an Organization Profile\"\n    },\n    \"default_packages\": {\n      \"type\": \"string\",\n      \"description\": \"Default packages of the notebook\"\n    },\n    \"user_packages\": {\n      \"type\": \"string\",\n      \"description\": \"User packages of the notebook\"\n    },\n    \"runtime_name\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime to run the Streamlit or Notebook on.  If this is not set, the warehouse is assumed\"\n    },\n    \"compute_pool\": {\n      \"type\": \"string\",\n      \"description\": \"Compute pool name where the snowservice runs\"\n    },\n    \"import_urls\": {\n      \"type\": \"array\",\n      \"description\": \"List of urls\"\n    },\n    \"external_access_integrations\": {\n      \"type\": \"array\",\n      \"description\": \"List of external access integrations attached to this function\"\n    },\n    \"external_access_secrets\": {\n      \"type\": \"string\",\n      \"description\": \"Secrets\
  \ to be used with this function for external access\"\n    },\n    \"idle_auto_shutdown_time_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Sets the time in seconds for when to shutdown an idle Notebook.\"\n    },\n    \"live_version_location_uri\": {\n      \"type\": \"string\",\n      \"description\": \"The current version location\"\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the budget if the notebook is monitored by a budget\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notebook-notebook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Notebook
---
