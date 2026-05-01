---
description: The values to filter results from the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventsForOrganization.html">DescribeEventsForOrganization</a> operation.
layout: schema
name: OrganizationEventFilter
properties_list:
- description: ''
  name: eventTypeCodes
  type: object
- description: ''
  name: awsAccountIds
  type: object
- description: ''
  name: services
  type: object
- description: ''
  name: regions
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: lastUpdatedTime
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
  name: eventStatusCodes
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-organization-event-filter-schema.json
slug: health-organization-event-filter
source_filename: health-organization-event-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-organization-event-filter-schema.json\",\n  \"title\": \"OrganizationEventFilter\",\n  \"description\": \"The values to filter results from the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeEventsForOrganization.html\\\">DescribeEventsForOrganization</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventTypeCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventTypeList\"\n        },\n        {\n          \"description\": \"A list of unique identifiers for event types. For example, <code>\\\"AWS_EC2_SYSTEM_MAINTENANCE_EVENT\\\",\\\"AWS_RDS_MAINTENANCE_SCHEDULED\\\".</code> \"\n        }\n      ]\n    },\n    \"awsAccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/awsAccountIdsList\"\
  \n        },\n        {\n          \"description\": \"A list of 12-digit Amazon Web Services account numbers that contains the affected entities.\"\n        }\n      ]\n    },\n    \"services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/serviceList\"\n        },\n        {\n          \"description\": \"The Amazon Web Services services associated with the event. For example, <code>EC2</code>, <code>RDS</code>.\"\n        }\n      ]\n    },\n    \"regions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/regionList\"\n        },\n        {\n          \"description\": \"A list of Amazon Web Services Regions.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"$ref\": \"#/components/schemas/DateTimeRange\"\n    },\n    \"endTime\": {\n      \"$ref\": \"#/components/schemas/DateTimeRange\"\n    },\n    \"lastUpdatedTime\": {\n      \"$ref\": \"#/components/schemas/DateTimeRange\"\n    },\n    \"entityArns\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityArnList\"\n        },\n        {\n          \"description\": \"A list of entity ARNs (unique identifiers).\"\n        }\n      ]\n    },\n    \"entityValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityValueList\"\n        },\n        {\n          \"description\": \"A list of entity identifiers, such as EC2 instance IDs (i-34ab692e) or EBS volumes (vol-426ab23e).\"\n        }\n      ]\n    },\n    \"eventTypeCategories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventTypeCategoryList\"\n        },\n        {\n          \"description\": \"A list of event type category codes. Possible values are <code>issue</code>, <code>accountNotification</code>, or <code>scheduledChange</code>. Currently, the <code>investigation</code> value isn't supported at this time.\"\n        }\n      ]\n    },\n    \"eventStatusCodes\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/eventStatusCodeList\"\n        },\n        {\n          \"description\": \"A list of event status codes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-organization-event-filter-schema.json
tags:
- Health Monitoring
- Notifications
- Operations
- Service Status
title: OrganizationEventFilter
---
