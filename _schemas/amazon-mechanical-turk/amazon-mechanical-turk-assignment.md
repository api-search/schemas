---
description: The Assignment data structure represents a single assignment of a HIT to a Worker. The assignment tracks the Worker's efforts to complete the HIT, and contains the results for later retrieval.
layout: schema
name: Assignment
properties_list:
- description: ''
  name: AssignmentId
  type: object
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: HITId
  type: object
- description: ''
  name: AssignmentStatus
  type: object
- description: ''
  name: AutoApprovalTime
  type: object
- description: ''
  name: AcceptTime
  type: object
- description: ''
  name: SubmitTime
  type: object
- description: ''
  name: ApprovalTime
  type: object
- description: ''
  name: RejectionTime
  type: object
- description: ''
  name: Deadline
  type: object
- description: ''
  name: Answer
  type: object
- description: ''
  name: RequesterFeedback
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-assignment-schema.json
slug: amazon-mechanical-turk-assignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-assignment-schema.json\",\n  \"title\": \"Assignment\",\n  \"description\": \" The Assignment data structure represents a single assignment of a HIT to a Worker. The assignment tracks the Worker's efforts to complete the HIT, and contains the results for later retrieval. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssignmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" A unique identifier for the assignment.\"\n        }\n      ]\n    },\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \" The ID of the Worker who accepted the HIT.\"\n        }\n     \
  \ ]\n    },\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the HIT.\"\n        }\n      ]\n    },\n    \"AssignmentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssignmentStatus\"\n        },\n        {\n          \"description\": \" The status of the assignment.\"\n        }\n      ]\n    },\n    \"AutoApprovalTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" If results have been submitted, AutoApprovalTime is the date and time the results of the assignment results are considered Approved automatically if they have not already been explicitly approved or rejected by the Requester. This value is derived from the auto-approval delay specified by the Requester in the HIT. This value is omitted from the assignment if the Worker has\
  \ not yet submitted results.\"\n        }\n      ]\n    },\n    \"AcceptTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time the Worker accepted the assignment.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" If the Worker has submitted results, SubmitTime is the date and time the assignment was submitted. This value is omitted from the assignment if the Worker has not yet submitted results.\"\n        }\n      ]\n    },\n    \"ApprovalTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" If the Worker has submitted results and the Requester has approved the results, ApprovalTime is the date and time the Requester approved the results.\
  \ This value is omitted from the assignment if the Requester has not yet approved the results.\"\n        }\n      ]\n    },\n    \"RejectionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" If the Worker has submitted results and the Requester has rejected the results, RejectionTime is the date and time the Requester rejected the results.\"\n        }\n      ]\n    },\n    \"Deadline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time of the deadline for the assignment. This value is derived from the deadline specification for the HIT and the date and time the Worker accepted the HIT.\"\n        }\n      ]\n    },\n    \"Answer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The Worker's\
  \ answers submitted for the HIT contained in a QuestionFormAnswers document, if the Worker provides an answer. If the Worker does not provide any answers, Answer may contain a QuestionFormAnswers document, or Answer may be empty.\"\n        }\n      ]\n    },\n    \"RequesterFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The feedback string included with the call to the ApproveAssignment operation or the RejectAssignment operation, if the Requester approved or rejected the assignment and specified feedback.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-assignment-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: Assignment
---
