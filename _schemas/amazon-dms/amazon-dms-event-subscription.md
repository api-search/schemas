---
description: Describes an event notification subscription created by the <code>CreateEventSubscription</code> operation.
layout: schema
name: EventSubscription
properties_list:
- description: ''
  name: CustomerAwsId
  type: object
- description: ''
  name: CustSubscriptionId
  type: object
- description: ''
  name: SnsTopicArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SubscriptionCreationTime
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: SourceIdsList
  type: object
- description: ''
  name: EventCategoriesList
  type: object
- description: ''
  name: Enabled
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-event-subscription-schema.json
slug: amazon-dms-event-subscription
source_filename: amazon-dms-event-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-event-subscription-schema.json\",\n  \"title\": \"EventSubscription\",\n  \"description\": \"Describes an event notification subscription created by the <code>CreateEventSubscription</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomerAwsId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Web Services customer account associated with the DMS event notification subscription.\"\n        }\n      ]\n    },\n    \"CustSubscriptionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The DMS event notification subscription Id.\"\n        }\n      ]\n    },\n    \"SnsTopicArn\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The topic ARN of the DMS event notification subscription.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The status of the DMS event notification subscription.</p> <p>Constraints:</p> <p>Can be one of the following: creating | modifying | deleting | active | no-permission | topic-not-exist</p> <p>The status \\\"no-permission\\\" indicates that DMS no longer has permission to post to the SNS topic. The status \\\"topic-not-exist\\\" indicates that the topic was deleted after the subscription was created.</p>\"\n        }\n      ]\n    },\n    \"SubscriptionCreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The\
  \ time the DMS event notification subscription was created.\"\n        }\n      ]\n    },\n    \"SourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> The type of DMS resource that generates events. </p> <p>Valid values: replication-instance | replication-server | security-group | replication-task</p>\"\n        }\n      ]\n    },\n    \"SourceIdsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceIdsList\"\n        },\n        {\n          \"description\": \"A list of source Ids for the event subscription.\"\n        }\n      ]\n    },\n    \"EventCategoriesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventCategoriesList\"\n        },\n        {\n          \"description\": \"A lists of event categories.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Boolean value that indicates if the event subscription is enabled.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-event-subscription-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: EventSubscription
---
