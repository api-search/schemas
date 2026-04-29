---
description: A user object. *New in version 2.1.0*
layout: schema
name: UserCollectionItem
properties_list:
- description: Whether the user is active
  name: active
  type: boolean
- description: The date user was changed
  name: changed_on
  type: string
- description: The date user was created
  name: created_on
  type: string
- description: The user's email. *Changed in version 2.2.0*&#58; A minimum character length requirement ('minLength') is added.
  name: email
  type: string
- description: The number of times the login failed
  name: failed_login_count
  type: integer
- description: The user's first name. *Changed in version 2.4.0*&#58; The requirement for this to be non-empty was removed.
  name: first_name
  type: string
- description: The last user login
  name: last_login
  type: string
- description: The user's last name. *Changed in version 2.4.0*&#58; The requirement for this to be non-empty was removed.
  name: last_name
  type: string
- description: The login count
  name: login_count
  type: integer
- description: User roles. *Changed in version 2.2.0*&#58; Field is no longer read-only.
  name: roles
  type: array
- description: The username. *Changed in version 2.2.0*&#58; A minimum character length requirement ('minLength') is added.
  name: username
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-user-collection-item-schema.json
slug: openapi.yaml-user-collection-item
source_filename: openapi.yaml-user-collection-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-user-collection-item-schema.json\",\n  \"title\": \"UserCollectionItem\",\n  \"description\": \"A user object.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"description\": \"Whether the user is active\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"changed_on\": {\n      \"description\": \"The date user was changed\",\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"created_on\": {\n      \"description\": \"The date user was created\",\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"description\":\
  \ \"The user's email.\\n\\n*Changed in version 2.2.0*&#58; A minimum character length requirement ('minLength') is added.\\n\",\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"failed_login_count\": {\n      \"description\": \"The number of times the login failed\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"first_name\": {\n      \"description\": \"The user's first name.\\n\\n*Changed in version 2.4.0*&#58; The requirement for this to be non-empty was removed.\\n\",\n      \"type\": \"string\"\n    },\n    \"last_login\": {\n      \"description\": \"The last user login\",\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"last_name\": {\n      \"description\": \"The user's last name.\\n\\n*Changed in version 2.4.0*&#58; The requirement for this to be non-empty was removed.\\n\",\n      \"type\": \"string\"\n    },\n    \"login_count\"\
  : {\n      \"description\": \"The login count\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"roles\": {\n      \"description\": \"User roles.\\n\\n*Changed in version 2.2.0*&#58; Field is no longer read-only.\\n\",\n      \"items\": {\n        \"nullable\": true,\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"username\": {\n      \"description\": \"The username.\\n\\n*Changed in version 2.2.0*&#58; A minimum character length requirement ('minLength') is added.\\n\",\n      \"minLength\": 1,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-user-collection-item-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: UserCollectionItem
---
