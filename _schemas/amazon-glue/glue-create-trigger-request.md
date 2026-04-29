---
description: CreateTriggerRequest schema from Amazon Glue API
layout: schema
name: CreateTriggerRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: WorkflowName
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Schedule
  type: object
- description: ''
  name: Predicate
  type: object
- description: ''
  name: Actions
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: StartOnCreation
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: EventBatchingCondition
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-trigger-request-schema.json
slug: glue-create-trigger-request
source_filename: glue-create-trigger-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-trigger-request-schema.json\",\n  \"title\": \"CreateTriggerRequest\",\n  \"description\": \"CreateTriggerRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the trigger.\"\n        }\n      ]\n    },\n    \"WorkflowName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the workflow associated with the trigger.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerType\"\n        },\n        {\n          \"description\"\
  : \"The type of the new trigger.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"<p>A <code>cron</code> expression used to specify the schedule (see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-data-warehouse-schedule.html\\\">Time-Based Schedules for Jobs and Crawlers</a>. For example, to run something every day at 12:15 UTC, you would specify: <code>cron(15 12 * * ? *)</code>.</p> <p>This field is required when the trigger type is SCHEDULED.</p>\"\n        }\n      ]\n    },\n    \"Predicate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Predicate\"\n        },\n        {\n          \"description\": \"<p>A predicate to specify when the new trigger should fire.</p> <p>This field is required when the trigger type is <code>CONDITIONAL</code>.</p>\"\n        }\n      ]\n    },\n    \"Actions\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionList\"\n        },\n        {\n          \"description\": \"The actions initiated by this trigger when it fires.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of the new trigger.\"\n        }\n      ]\n    },\n    \"StartOnCreation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanValue\"\n        },\n        {\n          \"description\": \"Set to <code>true</code> to start <code>SCHEDULED</code> and <code>CONDITIONAL</code> triggers when created. True is not supported for <code>ON_DEMAND</code> triggers.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags to\
  \ use with this trigger. You may use tags to limit access to the trigger. For more information about tags in Glue, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-tags.html\\\">Amazon Web Services Tags in Glue</a> in the developer guide. \"\n        }\n      ]\n    },\n    \"EventBatchingCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventBatchingCondition\"\n        },\n        {\n          \"description\": \"Batch condition that must be met (specified number of events received or batch time window expired) before EventBridge event trigger fires.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Type\",\n    \"Actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-trigger-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateTriggerRequest
---
