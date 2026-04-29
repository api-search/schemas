---
description: The values to use to filter results from the <a href="https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeAffectedEntities.html">DescribeAffectedEntities</a> operation.
layout: schema
name: EntityFilter
properties_list:
- description: ''
  name: eventArns
  type: object
- description: ''
  name: entityArns
  type: object
- description: ''
  name: entityValues
  type: object
- description: ''
  name: lastUpdatedTimes
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: statusCodes
  type: object
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-entity-filter-schema.json
slug: health-entity-filter
source_filename: health-entity-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-entity-filter-schema.json\",\n  \"title\": \"EntityFilter\",\n  \"description\": \"The values to use to filter results from the <a href=\\\"https://docs.aws.amazon.com/health/latest/APIReference/API_DescribeAffectedEntities.html\\\">DescribeAffectedEntities</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventArnList\"\n        },\n        {\n          \"description\": \"A list of event ARNs (unique identifiers). For example: <code>\\\"arn:aws:health:us-east-1::event/EC2/EC2_INSTANCE_RETIREMENT_SCHEDULED/EC2_INSTANCE_RETIREMENT_SCHEDULED_ABC123-CDE456\\\", \\\"arn:aws:health:us-west-1::event/EBS/AWS_EBS_LOST_VOLUME/AWS_EBS_LOST_VOLUME_CHI789_JKL101\\\"</code> \"\n        }\n \
  \     ]\n    },\n    \"entityArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityArnList\"\n        },\n        {\n          \"description\": \"A list of entity ARNs (unique identifiers).\"\n        }\n      ]\n    },\n    \"entityValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityValueList\"\n        },\n        {\n          \"description\": \"A list of IDs for affected entities.\"\n        }\n      ]\n    },\n    \"lastUpdatedTimes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/dateTimeRangeList\"\n        },\n        {\n          \"description\": \"A list of the most recent dates and times that the entity was updated.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/tagFilter\"\n        },\n        {\n          \"description\": \"<p>A map of entity tags attached to the affected entity.</p> <note> <p>Currently,\
  \ the <code>tags</code> property isn't supported.</p> </note>\"\n        }\n      ]\n    },\n    \"statusCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/entityStatusCodeList\"\n        },\n        {\n          \"description\": \"A list of entity status codes (<code>IMPAIRED</code>, <code>UNIMPAIRED</code>, or <code>UNKNOWN</code>).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-entity-filter-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EntityFilter
---
