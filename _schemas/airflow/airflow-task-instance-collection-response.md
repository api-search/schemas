---
description: 'Task instance collection response supporting both offset and cursor pagination. A single flat model is used instead of a discriminated union (``Annotated[Offset | Cursor, Field(discriminator=...)]``) because the OpenAPI ``oneOf`` + ``discriminator`` construct is not handled correctly by ``@hey-api/openapi-ts`` / ``@7nohe/openapi-react-query-codegen``: return types degrade to ``unknown`` in JSDoc and can produce incorrect TypeScript types (see hey-api/openapi-ts#1613, #3270).'
layout: schema
name: TaskInstanceCollectionResponse
properties_list:
- description: ''
  name: task_instances
  type: array
- description: Total number of matching items. Populated for offset pagination, ``null`` when using cursor pagination.
  name: total_entries
  type: object
- description: Token pointing to the next page. Populated for cursor pagination, ``null`` when using offset pagination or when there is no next page.
  name: next_cursor
  type: object
- description: Token pointing to the previous page. Populated for cursor pagination, ``null`` when using offset pagination or when on the first page.
  name: previous_cursor
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-instance-collection-response-schema.json
slug: airflow-task-instance-collection-response
source_filename: airflow-task-instance-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-collection-response-schema.json\",\n  \"title\": \"TaskInstanceCollectionResponse\",\n  \"description\": \"Task instance collection response supporting both offset and cursor pagination.\\n\\nA single flat model is used instead of a discriminated union\\n(``Annotated[Offset | Cursor, Field(discriminator=...)]``) because\\nthe OpenAPI ``oneOf`` + ``discriminator`` construct is not handled\\ncorrectly by ``@hey-api/openapi-ts`` / ``@7nohe/openapi-react-query-codegen``:\\nreturn types degrade to ``unknown`` in JSDoc and can produce\\nincorrect TypeScript types (see hey-api/openapi-ts#1613, #3270).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"task_instances\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskInstanceResponse\"\n      },\n      \"type\": \"array\"\
  ,\n      \"title\": \"Task Instances\"\n    },\n    \"total_entries\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Total Entries\",\n      \"description\": \"Total number of matching items. Populated for offset pagination, ``null`` when using cursor pagination.\"\n    },\n    \"next_cursor\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Next Cursor\",\n      \"description\": \"Token pointing to the next page. Populated for cursor pagination, ``null`` when using offset pagination or when there is no next page.\"\n    },\n    \"previous_cursor\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Previous Cursor\",\n      \"description\": \"Token pointing\
  \ to the previous page. Populated for cursor pagination, ``null`` when using offset pagination or when on the first page.\"\n    }\n  },\n  \"required\": [\n    \"task_instances\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskInstanceCollectionResponse
---
