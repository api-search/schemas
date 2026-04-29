---
description: A version of an integration containing the complete configuration including triggers, tasks, and parameters for automating workflows within Google Cloud.
layout: schema
name: Apigee Integration Version
properties_list:
- description: Output only. Resource name of the version.
  name: name
  type: string
- description: Description of the integration version.
  name: description
  type: string
- description: List of task configurations in the integration.
  name: taskConfigs
  type: array
- description: List of trigger configurations.
  name: triggerConfigs
  type: array
- description: Parameters used by the integration.
  name: integrationParameters
  type: array
- description: State of the integration version.
  name: state
  type: string
- description: Output only. Auto-incrementing snapshot number.
  name: snapshotNumber
  type: string
- description: Output only. Time the version was created.
  name: createTime
  type: string
- description: Output only. Email of the last modifier.
  name: lastModifierEmail
  type: string
- description: ID of the template this version was created from.
  name: parentTemplateId
  type: string
- description: User-defined label for the version.
  name: userLabel
  type: string
- description: Database persistence policy for execution logs.
  name: databasePersistencePolicy
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-integration-schema.json
slug: apigee-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-integration-schema.json\",\n  \"title\": \"Apigee Integration Version\",\n  \"description\": \"A version of an integration containing the complete configuration including triggers, tasks, and parameters for automating workflows within Google Cloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Resource name of the version.\",\n      \"readOnly\": true\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the integration version.\"\n    },\n    \"taskConfigs\": {\n      \"type\": \"array\",\n      \"description\": \"List of task configurations in the integration.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TaskConfig\"\n      }\n    },\n    \"triggerConfigs\": {\n      \"type\": \"array\",\n      \"description\": \"List\
  \ of trigger configurations.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TriggerConfig\"\n      }\n    },\n    \"integrationParameters\": {\n      \"type\": \"array\",\n      \"description\": \"Parameters used by the integration.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/IntegrationParameter\"\n      }\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State of the integration version.\",\n      \"enum\": [\"INTEGRATION_STATE_UNSPECIFIED\", \"DRAFT\", \"ACTIVE\", \"ARCHIVED\", \"SNAPSHOT\"]\n    },\n    \"snapshotNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Auto-incrementing snapshot number.\",\n      \"readOnly\": true\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. Time the version was created.\",\n      \"readOnly\": true\n    },\n    \"lastModifierEmail\": {\n      \"type\": \"string\",\n      \"description\": \"Output\
  \ only. Email of the last modifier.\",\n      \"readOnly\": true\n    },\n    \"parentTemplateId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the template this version was created from.\"\n    },\n    \"userLabel\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined label for the version.\"\n    },\n    \"databasePersistencePolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Database persistence policy for execution logs.\",\n      \"enum\": [\"DATABASE_PERSISTENCE_POLICY_UNSPECIFIED\", \"DATABASE_PERSISTENCE_DISABLED\", \"DATABASE_PERSISTENCE_ASYNC\"]\n    }\n  },\n  \"$defs\": {\n    \"TaskConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for a task in an integration.\",\n      \"properties\": {\n        \"task\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the task.\"\n        },\n        \"taskId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique\
  \ ID of the task within the integration.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name for the task.\"\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"description\": \"Task parameters.\",\n          \"additionalProperties\": true\n        },\n        \"nextTasks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"taskId\": { \"type\": \"string\" },\n              \"condition\": { \"type\": \"string\" },\n              \"displayName\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"taskExecutionStrategy\": {\n          \"type\": \"string\",\n          \"enum\": [\"WHEN_ALL_SUCCEED\", \"WHEN_ANY_SUCCEED\", \"WHEN_ALL_TASKS_AND_CONDITIONS_SUCCEED\"]\n        },\n        \"failurePolicy\": {\n          \"type\": \"object\",\n          \"properties\": {\n         \
  \   \"retryStrategy\": {\n              \"type\": \"string\",\n              \"enum\": [\"RETRY_STRATEGY_UNSPECIFIED\", \"IGNORE\", \"NONE\", \"FATAL\", \"FIXED_INTERVAL\", \"LINEAR_BACKOFF\", \"EXPONENTIAL_BACKOFF\", \"RESTART_INTEGRATION_WITH_BACKOFF\"]\n            },\n            \"maxRetries\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      },\n      \"required\": [\"task\", \"taskId\"]\n    },\n    \"TriggerConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for a trigger that starts an integration.\",\n      \"properties\": {\n        \"trigger\": { \"type\": \"string\" },\n        \"triggerId\": { \"type\": \"string\" },\n        \"label\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"triggerType\": {\n          \"type\": \"string\",\n          \"enum\": [\"TRIGGER_TYPE_UNSPECIFIED\", \"CRON\", \"API\", \"SFDC_CHANNEL\", \"CLOUD_PUBSUB_EXTERNAL\", \"SFDC_CDC_CHANNEL\"\
  , \"CLOUD_SCHEDULER\", \"INTEGRATION_CONNECTOR_TRIGGER\"]\n        },\n        \"startTasks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"taskId\": { \"type\": \"string\" },\n              \"condition\": { \"type\": \"string\" }\n            }\n          }\n        }\n      },\n      \"required\": [\"triggerId\"]\n    },\n    \"IntegrationParameter\": {\n      \"type\": \"object\",\n      \"description\": \"A parameter used in an integration.\",\n      \"properties\": {\n        \"key\": { \"type\": \"string\" },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"enum\": [\"INTEGRATION_PARAMETER_DATA_TYPE_UNSPECIFIED\", \"STRING_VALUE\", \"INT_VALUE\", \"DOUBLE_VALUE\", \"BOOLEAN_VALUE\", \"STRING_ARRAY\", \"INT_ARRAY\", \"DOUBLE_ARRAY\", \"BOOLEAN_ARRAY\", \"JSON_VALUE\", \"PROTO_VALUE\", \"PROTO_ARRAY\"]\n        },\n        \"inputOutputType\": {\n          \"type\"\
  : \"string\",\n          \"enum\": [\"IN_OUT_TYPE_UNSPECIFIED\", \"IN\", \"OUT\", \"IN_OUT\"]\n        },\n        \"isTransient\": { \"type\": \"boolean\" },\n        \"producer\": { \"type\": \"string\" }\n      },\n      \"required\": [\"key\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-integration-schema.json
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee Integration Version
---
