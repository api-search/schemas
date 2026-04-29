---
description: The HIT data structure represents a single HIT, including all the information necessary for a Worker to accept and complete the HIT.
layout: schema
name: HIT
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: HITTypeId
  type: object
- description: ''
  name: HITGroupId
  type: object
- description: ''
  name: HITLayoutId
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Question
  type: object
- description: ''
  name: Keywords
  type: object
- description: ''
  name: HITStatus
  type: object
- description: ''
  name: MaxAssignments
  type: object
- description: ''
  name: Reward
  type: object
- description: ''
  name: AutoApprovalDelayInSeconds
  type: object
- description: ''
  name: Expiration
  type: object
- description: ''
  name: AssignmentDurationInSeconds
  type: object
- description: ''
  name: RequesterAnnotation
  type: object
- description: ''
  name: QualificationRequirements
  type: object
- description: ''
  name: HITReviewStatus
  type: object
- description: ''
  name: NumberOfAssignmentsPending
  type: object
- description: ''
  name: NumberOfAssignmentsAvailable
  type: object
- description: ''
  name: NumberOfAssignmentsCompleted
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-hit-schema.json
slug: amazon-mechanical-turk-hit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-hit-schema.json\",\n  \"title\": \"HIT\",\n  \"description\": \" The HIT data structure represents a single HIT, including all the information necessary for a Worker to accept and complete the HIT.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" A unique identifier for the HIT.\"\n        }\n      ]\n    },\n    \"HITTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the HIT type of this HIT\"\n        }\n      ]\n    },\n    \"HITGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\
  \n        },\n        {\n          \"description\": \" The ID of the HIT Group of this HIT.\"\n        }\n      ]\n    },\n    \"HITLayoutId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the HIT Layout of this HIT.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time the HIT was created.\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The title of the HIT.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A general description of the HIT.\"\n   \
  \     }\n      ]\n    },\n    \"Question\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The data the Worker completing the HIT uses produce the results. This is either either a QuestionForm, HTMLQuestion or an ExternalQuestion data structure.\"\n        }\n      ]\n    },\n    \"Keywords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" One or more words or phrases that describe the HIT, separated by commas. Search terms similar to the keywords of a HIT are more likely to have the HIT in the search results.\"\n        }\n      ]\n    },\n    \"HITStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HITStatus\"\n        },\n        {\n          \"description\": \"The status of the HIT and its assignments. Valid Values are Assignable | Unassignable | Reviewable | Reviewing\
  \ | Disposed. \"\n        }\n      ]\n    },\n    \"MaxAssignments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of times the HIT can be accepted and completed before the HIT becomes unavailable. \"\n        }\n      ]\n    },\n    \"Reward\": {\n      \"$ref\": \"#/components/schemas/CurrencyAmount\"\n    },\n    \"AutoApprovalDelayInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The amount of time, in seconds, after the Worker submits an assignment for the HIT that the results are automatically approved by Amazon Mechanical Turk. This is the amount of time the Requester has to reject an assignment submitted by a Worker before the assignment is auto-approved and the Worker is paid. \"\n        }\n      ]\n    },\n    \"Expiration\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the HIT expires.\"\n        }\n      ]\n    },\n    \"AssignmentDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The length of time, in seconds, that a Worker has to complete the HIT after accepting it.\"\n        }\n      ]\n    },\n    \"RequesterAnnotation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" An arbitrary data field the Requester who created the HIT can use. This field is visible only to the creator of the HIT.\"\n        }\n      ]\n    },\n    \"QualificationRequirements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationRequirementList\"\n        },\n        {\n          \"description\": \" Conditions that a Worker's\
  \ Qualifications must meet in order to accept the HIT. A HIT can have between zero and ten Qualification requirements. All requirements must be met in order for a Worker to accept the HIT. Additionally, other actions can be restricted using the <code>ActionsGuarded</code> field on each <code>QualificationRequirement</code> structure. \"\n        }\n      ]\n    },\n    \"HITReviewStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HITReviewStatus\"\n        },\n        {\n          \"description\": \" Indicates the review status of the HIT. Valid Values are NotReviewed | MarkedForReview | ReviewedAppropriate | ReviewedInappropriate.\"\n        }\n      ]\n    },\n    \"NumberOfAssignmentsPending\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of assignments for this HIT that are being previewed or have been accepted by Workers, but have not yet been\
  \ submitted, returned, or abandoned.\"\n        }\n      ]\n    },\n    \"NumberOfAssignmentsAvailable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of assignments for this HIT that are available for Workers to accept.\"\n        }\n      ]\n    },\n    \"NumberOfAssignmentsCompleted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of assignments for this HIT that have been approved or rejected.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-hit-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: HIT
---
