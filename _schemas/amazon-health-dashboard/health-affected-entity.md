---
description: Information about an entity that is affected by a Health event.
layout: schema
name: AffectedEntity
properties_list:
- description: ''
  name: entityArn
  type: object
- description: ''
  name: eventArn
  type: object
- description: ''
  name: entityValue
  type: object
- description: ''
  name: entityUrl
  type: object
- description: ''
  name: awsAccountId
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
- description: ''
  name: statusCode
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-affected-entity-schema.json
slug: health-affected-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-affected-entity-schema.json\",\n  \"title\": \"AffectedEntity\",\n  \"description\": \"Information about an entity that is affected by a Health event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityArn\"\n        },\n        {\n          \"description\": \"The unique identifier for the entity. Format: <code>arn:aws:health:<i>entity-region</i>:<i>aws-account</i>:entity/<i>entity-id</i> </code>. Example: <code>arn:aws:health:us-east-1:111222333444:entity/AVh5GGT7ul1arKr1sE1K</code> \"\n        }\n      ]\n    },\n    \"eventArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArn\"\n        },\n        {\n          \"description\": \"<p>The unique identifier\
  \ for the event. The event ARN has the <code>arn:aws:health:<i>event-region</i>::event/<i>SERVICE</i>/<i>EVENT_TYPE_CODE</i>/<i>EVENT_TYPE_PLUS_ID</i> </code> format.</p> <p>For example, an event ARN might look like the following:</p> <p> <code>arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-DEF456</code> </p>\"\n        }\n      ]\n    },\n    \"entityValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityValue\"\n        },\n        {\n          \"description\": \"The ID of the affected entity.\"\n        }\n      ]\n    },\n    \"entityUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityUrl\"\n        },\n        {\n          \"description\": \"The URL of the affected entity.\"\n        }\n      ]\n    },\n    \"awsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/accountId\"\n        },\n        {\n       \
  \   \"description\": \"The 12-digit Amazon Web Services account number that contains the affected entity.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The most recent time that the entity was updated.\"\n        }\n      ]\n    },\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityStatusCode\"\n        },\n        {\n          \"description\": \"The most recent status of the entity affected by the event. The possible values are <code>IMPAIRED</code>, <code>UNIMPAIRED</code>, and <code>UNKNOWN</code>.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/tagSet\"\n        },\n        {\n          \"description\": \"<p>A map of entity tags attached to the affected entity.</p> <note> <p>Currently, the <code>tags</code>\
  \ property isn't supported.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-affected-entity-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: AffectedEntity
---
