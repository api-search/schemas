---
description: Schema representing a work item within the Automation Anywhere Workload Management system. A work item is a single unit of data queued for processing by an RPA bot, with a typed payload defined by the queue's work item model and lifecycle status tracking from creation through completion.
layout: schema
name: Automation Anywhere Work Item
properties_list:
- description: Unique numeric identifier of the work item assigned by the Control Room upon creation
  name: id
  type: integer
- description: Numeric ID of the Workload Management queue this work item belongs to
  name: queueId
  type: integer
- description: Key-value data payload of the work item. Keys are attribute names defined in the queue's work item model; values are the actual data to be processed by the bot.
  name: json
  type: object
- description: Current lifecycle status of the work item indicating where it is in the processing pipeline
  name: status
  type: string
- description: Processing outcome recorded by the bot upon completing or failing this work item
  name: result
  type: string
- description: 'Display column 1: a human-readable label extracted from the work item data for display in the Control Room queue viewer'
  name: col1
  type: string
- description: 'Display column 2: a secondary human-readable label extracted from the work item data'
  name: col2
  type: string
- description: 'Display column 3: a tertiary human-readable label extracted from the work item data'
  name: col3
  type: string
- description: Numeric ID of the Bot Runner device that processed or is currently processing this work item
  name: deviceId
  type: integer
- description: Numeric ID of the user account under which the processing bot executed on the device
  name: deviceUserId
  type: integer
- description: Deployment ID (UUID) of the automation that processed this work item, linking back to the deployment record
  name: automationId
  type: string
- description: Identifier of the job execution associated with processing this work item
  name: jobExecutionId
  type: string
- description: ISO 8601 timestamp when the bot began processing this work item
  name: startTime
  type: string
- description: ISO 8601 timestamp when bot processing of this work item completed
  name: endTime
  type: string
- description: ISO 8601 timestamp until which this work item is deferred; the bot will not pick it up before this time
  name: deferredUntil
  type: string
- description: ISO 8601 timestamp when the work item was last paused during processing
  name: lastPausedTime
  type: string
- description: Total time in seconds this work item was in a paused state
  name: totalPausedTime
  type: integer
- description: Optional free-text comment added by the processing bot or a human operator
  name: comment
  type: string
- description: Error message recorded when the work item processing failed, for debugging and retry decisions
  name: error
  type: string
- description: Number of times this work item has been automatically retried after failure
  name: retryCount
  type: integer
- description: Hash of the work item data used for duplicate detection when disallowDuplicate is enabled on the queue
  name: hashCode
  type: integer
- description: Optimistic concurrency control version number; must match the server value when updating
  name: version
  type: integer
- description: UUID of the tenant in a multi-tenant Control Room deployment
  name: tenantUuid
  type: string
- description: Numeric ID of the user who created this work item
  name: createdBy
  type: integer
- description: ISO 8601 timestamp when this work item was added to the queue
  name: createdOn
  type: string
- description: Numeric ID of the user who last modified this work item
  name: updatedBy
  type: integer
- description: ISO 8601 timestamp of the last status or data update to this work item
  name: updatedOn
  type: string
provider_name: automation-anywhere
provider_slug: automation-anywhere
schema_file: json-schema/automation-anywhere-work-item-schema.json
slug: automation-anywhere-work-item
source_filename: automation-anywhere-work-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://automationanywhere.com/schemas/work-item.json\",\n  \"title\": \"Automation Anywhere Work Item\",\n  \"description\": \"Schema representing a work item within the Automation Anywhere Workload Management system. A work item is a single unit of data queued for processing by an RPA bot, with a typed payload defined by the queue's work item model and lifecycle status tracking from creation through completion.\",\n  \"type\": \"object\",\n  \"required\": [\"queueId\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier of the work item assigned by the Control Room upon creation\"\n    },\n    \"queueId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric ID of the Workload Management queue this work item belongs to\"\n    },\n    \"json\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value data\
  \ payload of the work item. Keys are attribute names defined in the queue's work item model; values are the actual data to be processed by the bot.\",\n      \"additionalProperties\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the work item indicating where it is in the processing pipeline\",\n      \"enum\": [\"NEW\", \"IN_PROGRESS\", \"FAILED\", \"COMPLETE\", \"DEFERRED\"]\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"Processing outcome recorded by the bot upon completing or failing this work item\",\n      \"enum\": [\"SUCCESS\", \"FAILURE\"]\n    },\n    \"col1\": {\n      \"type\": \"string\",\n      \"description\": \"Display column 1: a human-readable label extracted from the work item data for display in the Control Room queue viewer\"\n    },\n    \"col2\": {\n      \"type\": \"string\",\n      \"description\": \"Display column 2: a secondary human-readable label extracted\
  \ from the work item data\"\n    },\n    \"col3\": {\n      \"type\": \"string\",\n      \"description\": \"Display column 3: a tertiary human-readable label extracted from the work item data\"\n    },\n    \"deviceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric ID of the Bot Runner device that processed or is currently processing this work item\"\n    },\n    \"deviceUserId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric ID of the user account under which the processing bot executed on the device\"\n    },\n    \"automationId\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment ID (UUID) of the automation that processed this work item, linking back to the deployment record\"\n    },\n    \"jobExecutionId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the job execution associated with processing this work item\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"ISO 8601 timestamp when the bot began processing this work item\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when bot processing of this work item completed\"\n    },\n    \"deferredUntil\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp until which this work item is deferred; the bot will not pick it up before this time\"\n    },\n    \"lastPausedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the work item was last paused during processing\"\n    },\n    \"totalPausedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Total time in seconds this work item was in a paused state\",\n      \"minimum\": 0\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional free-text comment added by\
  \ the processing bot or a human operator\",\n      \"maxLength\": 2000\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message recorded when the work item processing failed, for debugging and retry decisions\"\n    },\n    \"retryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times this work item has been automatically retried after failure\",\n      \"minimum\": 0\n    },\n    \"hashCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Hash of the work item data used for duplicate detection when disallowDuplicate is enabled on the queue\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Optimistic concurrency control version number; must match the server value when updating\"\n    },\n    \"tenantUuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"UUID of the tenant in a multi-tenant Control Room deployment\"\n    },\n    \"createdBy\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Numeric ID of the user who created this work item\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when this work item was added to the queue\"\n    },\n    \"updatedBy\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric ID of the user who last modified this work item\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last status or data update to this work item\"\n    }\n  },\n  \"$defs\": {\n    \"WorkItemModel\": {\n      \"type\": \"object\",\n      \"description\": \"Schema definition for work items in a queue, specifying the named attributes and their data types that each work item must contain\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"Unique identifier of the work item model\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name for the work item model\"\n        },\n        \"attributes\": {\n          \"type\": \"array\",\n          \"description\": \"Ordered list of attribute definitions that form the work item data schema\",\n          \"items\": {\n            \"$ref\": \"#/$defs/WorkItemAttribute\"\n          }\n        },\n        \"createdOn\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when this model was created\"\n        },\n        \"updatedOn\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp of the last modification to this model\"\n        }\n      }\n    },\n    \"WorkItemAttribute\": {\n      \"type\": \"object\",\n      \"description\": \"A single named attribute definition\
  \ within a work item model\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of this attribute\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Attribute name used as the key in work item JSON payloads\",\n          \"minLength\": 1,\n          \"maxLength\": 100\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of values stored in this attribute\",\n          \"enum\": [\"TEXT\", \"NUMBER\", \"DATE\", \"BOOLEAN\"]\n        },\n        \"isRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this attribute must be provided when creating a work item\"\n        }\n      }\n    },\n    \"Queue\": {\n      \"type\": \"object\",\n      \"description\": \"A work item queue configuration in the Workload Management system\",\n      \"required\"\
  : [\"name\", \"workItemModelId\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the queue\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name for the queue\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Optional description of the queue's business purpose\"\n        },\n        \"workItemModelId\": {\n          \"type\": \"integer\",\n          \"description\": \"ID of the work item model defining the data schema for items in this queue\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current operational status of the queue\",\n          \"enum\": [\"ACTIVE\", \"INACTIVE\"]\n        },\n        \"reactivationThreshold\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Percentage of remaining work items below which the queue triggers reactivation of bot processing\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"disallowDuplicate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to reject work items that have the same data hash as an existing item in the queue\"\n        },\n        \"autoRetryLimit\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of automatic retries for failed work items before they are marked as permanently failed\",\n          \"minimum\": 0,\n          \"maximum\": 10\n        },\n        \"workItemProcessingOrders\": {\n          \"type\": \"array\",\n          \"description\": \"Ordered list of attribute names by which work items are prioritized for processing\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/json-schema/automation-anywhere-work-item-schema.json
tags: []
title: Automation Anywhere Work Item
---
