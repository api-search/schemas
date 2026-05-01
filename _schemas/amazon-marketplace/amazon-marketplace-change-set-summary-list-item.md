---
description: A summary of a change set returned in a list of change sets when the <code>ListChangeSets</code> action is called.
layout: schema
name: ChangeSetSummaryListItem
properties_list:
- description: ''
  name: ChangeSetId
  type: object
- description: ''
  name: ChangeSetArn
  type: object
- description: ''
  name: ChangeSetName
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: EntityIdList
  type: object
- description: ''
  name: FailureCode
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-change-set-summary-list-item-schema.json
slug: amazon-marketplace-change-set-summary-list-item
source_filename: amazon-marketplace-change-set-summary-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-change-set-summary-list-item-schema.json\",\n  \"title\": \"ChangeSetSummaryListItem\",\n  \"description\": \"A summary of a change set returned in a list of change sets when the <code>ListChangeSets</code> action is called.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier for a change set.\"\n        }\n      ]\n    },\n    \"ChangeSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN associated with the unique identifier for the change set referenced in this request.\"\n        }\n      ]\n    },\n\
  \    \"ChangeSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeSetName\"\n        },\n        {\n          \"description\": \"The non-unique name for the change set.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeISO8601\"\n        },\n        {\n          \"description\": \"The time, in ISO 8601 format (2018-02-27T13:45:22Z), when the change set was started.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeISO8601\"\n        },\n        {\n          \"description\": \"The time, in ISO 8601 format (2018-02-27T13:45:22Z), when the change set was finished.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeStatus\"\n        },\n        {\n          \"description\": \"The current status of the change\
  \ set.\"\n        }\n      ]\n    },\n    \"EntityIdList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdList\"\n        },\n        {\n          \"description\": \"This object is a list of entity IDs (string) that are a part of a change set. The entity ID list is a maximum of 20 entities. It must contain at least one entity.\"\n        }\n      ]\n    },\n    \"FailureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureCode\"\n        },\n        {\n          \"description\": \"Returned if the change set is in <code>FAILED</code> status. Can be either <code>CLIENT_ERROR</code>, which means that there are issues with the request (see the <code>ErrorDetailList</code> of <code>DescribeChangeSet</code>), or <code>SERVER_FAULT</code>, which means that there is a problem in the system, and you should retry your request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-change-set-summary-list-item-schema.json
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ChangeSetSummaryListItem
---
