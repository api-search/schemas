---
description: The values to use to filter results from the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEvents.html">DescribeEvents</a> and <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventAggregates.html">DescribeEventAggregates</a> operations.
layout: schema
name: EventFilter
properties_list:
- description: ''
  name: eventArns
  type: object
- description: ''
  name: eventTypeCodes
  type: object
- description: ''
  name: services
  type: object
- description: ''
  name: regions
  type: object
- description: ''
  name: availabilityZones
  type: object
- description: ''
  name: startTimes
  type: object
- description: ''
  name: endTimes
  type: object
- description: ''
  name: lastUpdatedTimes
  type: object
- description: ''
  name: entityArns
  type: object
- description: ''
  name: entityValues
  type: object
- description: ''
  name: eventTypeCategories
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: eventStatusCodes
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-filter-schema.json
slug: health-event-filter
source_filename: health-event-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-filter-schema.json\",\n  \"title\": \"EventFilter\",\n  \"description\": \"The values to use to filter results from the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEvents.html\\\">DescribeEvents</a> and <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventAggregates.html\\\">DescribeEventAggregates</a> operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArnList\"\n        },\n        {\n          \"description\": \"A list of event ARNs (unique identifiers). For example: <code>\\\"arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-CDE456\\\", \\\"arn:aws:health:us-west-1::event/EBS/AWS_EBS_LOST_VOLUME/AWS_EBS_LOST_VOLUME_CHI789_JKL101\\\
  \"</code> \"\n        }\n      ]\n    },\n    \"eventTypeCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventTypeList\"\n        },\n        {\n          \"description\": \"A list of unique identifiers for event types. For example, <code>\\\"AWS_EC2_SYSTEM_MAINTENANCE_EVENT\\\",\\\"AWS_RDS_MAINTENANCE_SCHEDULED\\\".</code> \"\n        }\n      ]\n    },\n    \"services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/serviceList\"\n        },\n        {\n          \"description\": \"The Amazon Web Services services associated with the event. For example, <code>EC2</code>, <code>RDS</code>.\"\n        }\n      ]\n    },\n    \"regions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/regionList\"\n        },\n        {\n          \"description\": \"A list of Amazon Web Services Regions.\"\n        }\n      ]\n    },\n    \"availabilityZones\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/availabilityZones\"\n        },\n        {\n          \"description\": \"A list of Amazon Web Services Availability Zones.\"\n        }\n      ]\n    },\n    \"startTimes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/dateTimeRangeList\"\n        },\n        {\n          \"description\": \"A list of dates and times that the event began.\"\n        }\n      ]\n    },\n    \"endTimes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/dateTimeRangeList\"\n        },\n        {\n          \"description\": \"A list of dates and times that the event ended.\"\n        }\n      ]\n    },\n    \"lastUpdatedTimes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/dateTimeRangeList\"\n        },\n        {\n          \"description\": \"A list of dates and times that the event was last updated.\"\n        }\n      ]\n    },\n    \"entityArns\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/entityArnList\"\n        },\n        {\n          \"description\": \"A list of entity ARNs (unique identifiers).\"\n        }\n      ]\n    },\n    \"entityValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityValueList\"\n        },\n        {\n          \"description\": \"A list of entity identifiers, such as EC2 instance IDs (<code>i-34ab692e</code>) or EBS volumes (<code>vol-426ab23e</code>).\"\n        }\n      ]\n    },\n    \"eventTypeCategories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventTypeCategoryList\"\n        },\n        {\n          \"description\": \"A list of event type category codes. Possible values are <code>issue</code>, <code>accountNotification</code>, or <code>scheduledChange</code>. Currently, the <code>investigation</code> value isn't supported at this time.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/tagFilter\"\n        },\n        {\n          \"description\": \"<p>A map of entity tags attached to the affected entity.</p> <note> <p>Currently, the <code>tags</code> property isn't supported.</p> </note>\"\n        }\n      ]\n    },\n    \"eventStatusCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventStatusCodeList\"\n        },\n        {\n          \"description\": \"A list of event status codes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-filter-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EventFilter
---
