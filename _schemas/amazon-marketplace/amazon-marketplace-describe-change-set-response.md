---
description: DescribeChangeSetResponse schema from Amazon Marketplace API
layout: schema
name: DescribeChangeSetResponse
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
  name: FailureCode
  type: object
- description: ''
  name: FailureDescription
  type: object
- description: ''
  name: ChangeSet
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-describe-change-set-response-schema.json
slug: amazon-marketplace-describe-change-set-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-describe-change-set-response-schema.json\",\n  \"title\": \"DescribeChangeSetResponse\",\n  \"description\": \"DescribeChangeSetResponse schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"Required. The unique identifier for the change set referenced in this request.\"\n        }\n      ]\n    },\n    \"ChangeSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN associated with the unique identifier for the change set referenced in this request.\"\n        }\n      ]\n    },\n    \"ChangeSetName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeSetName\"\n        },\n        {\n          \"description\": \"The optional name provided in the <code>StartChangeSet</code> request. If you do not provide a name, one is set by default.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeISO8601\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format (2018-02-27T13:45:22Z), the request started. \"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeISO8601\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format (2018-02-27T13:45:22Z), the request transitioned to a terminal state. The change cannot transition to a different state. Null if the request is not in a terminal state. \"\n        }\n      ]\n    },\n    \"Status\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeStatus\"\n        },\n        {\n          \"description\": \"The status of the change request.\"\n        }\n      ]\n    },\n    \"FailureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureCode\"\n        },\n        {\n          \"description\": \"Returned if the change set is in <code>FAILED</code> status. Can be either <code>CLIENT_ERROR</code>, which means that there are issues with the request (see the <code>ErrorDetailList</code>), or <code>SERVER_FAULT</code>, which means that there is a problem in the system, and you should retry your request.\"\n        }\n      ]\n    },\n    \"FailureDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExceptionMessageContent\"\n        },\n        {\n          \"description\": \"Returned if there is a failure on the change set, but that failure is not related to any of the changes\
  \ in the request.\"\n        }\n      ]\n    },\n    \"ChangeSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeSetDescription\"\n        },\n        {\n          \"description\": \"An array of <code>ChangeSummary</code> objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-describe-change-set-response-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: DescribeChangeSetResponse
---
