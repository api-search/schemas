---
description: CreateHITRequest schema from Amazon Mechanical Turk API
layout: schema
name: CreateHITRequest
properties_list:
- description: ''
  name: MaxAssignments
  type: object
- description: ''
  name: AutoApprovalDelayInSeconds
  type: object
- description: ''
  name: LifetimeInSeconds
  type: object
- description: ''
  name: AssignmentDurationInSeconds
  type: object
- description: ''
  name: Reward
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Keywords
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Question
  type: object
- description: ''
  name: RequesterAnnotation
  type: object
- description: ''
  name: QualificationRequirements
  type: object
- description: ''
  name: UniqueRequestToken
  type: object
- description: ''
  name: AssignmentReviewPolicy
  type: object
- description: ''
  name: HITReviewPolicy
  type: object
- description: ''
  name: HITLayoutId
  type: object
- description: ''
  name: HITLayoutParameters
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-create-hit-request-schema.json
slug: amazon-mechanical-turk-create-hit-request
source_filename: amazon-mechanical-turk-create-hit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-hit-request-schema.json\",\n  \"title\": \"CreateHITRequest\",\n  \"description\": \"CreateHITRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxAssignments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of times the HIT can be accepted and completed before the HIT becomes unavailable. \"\n        }\n      ]\n    },\n    \"AutoApprovalDelayInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The number of seconds after an assignment for the HIT has been submitted, after which the assignment is considered Approved\
  \ automatically unless the Requester explicitly rejects it. \"\n        }\n      ]\n    },\n    \"LifetimeInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" An amount of time, in seconds, after which the HIT is no longer available for users to accept. After the lifetime of the HIT elapses, the HIT no longer appears in HIT searches, even if not all of the assignments for the HIT have been accepted. \"\n        }\n      ]\n    },\n    \"AssignmentDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The amount of time, in seconds, that a Worker has to complete the HIT after accepting it. If a Worker does not complete the assignment within the specified duration, the assignment is considered abandoned. If the HIT is still active (that is, its lifetime has not elapsed), the assignment becomes\
  \ available for other users to find and accept. \"\n        }\n      ]\n    },\n    \"Reward\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrencyAmount\"\n        },\n        {\n          \"description\": \" The amount of money the Requester will pay a Worker for successfully completing the HIT. \"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The title of the HIT. A title should be short and descriptive about the kind of task the HIT contains. On the Amazon Mechanical Turk web site, the HIT title appears in search results, and everywhere the HIT is mentioned. \"\n        }\n      ]\n    },\n    \"Keywords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" One or more words or phrases that describe the HIT, separated by commas.\
  \ These words are used in searches to find HITs. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A general description of the HIT. A description includes detailed information about the kind of task the HIT contains. On the Amazon Mechanical Turk web site, the HIT description appears in the expanded view of search results, and in the HIT and assignment screens. A good description gives the user enough information to evaluate the HIT before accepting it. \"\n        }\n      ]\n    },\n    \"Question\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> The data the person completing the HIT uses to produce the results. </p> <p> Constraints: Must be a QuestionForm data structure, an ExternalQuestion data structure, or an HTMLQuestion data structure. The XML\
  \ question data must not be larger than 64 kilobytes (65,535 bytes) in size, including whitespace. </p> <p>Either a Question parameter or a HITLayoutId parameter must be provided.</p>\"\n        }\n      ]\n    },\n    \"RequesterAnnotation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> An arbitrary data field. The RequesterAnnotation parameter lets your application attach arbitrary data to the HIT for tracking purposes. For example, this parameter could be an identifier internal to the Requester's application that corresponds with the HIT. </p> <p> The RequesterAnnotation parameter for a HIT is only visible to the Requester who created the HIT. It is not shown to the Worker, or any other Requester. </p> <p> The RequesterAnnotation parameter may be different for each HIT you submit. It does not affect how your HITs are grouped. </p>\"\n        }\n      ]\n    },\n    \"QualificationRequirements\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationRequirementList\"\n        },\n        {\n          \"description\": \" Conditions that a Worker's Qualifications must meet in order to accept the HIT. A HIT can have between zero and ten Qualification requirements. All requirements must be met in order for a Worker to accept the HIT. Additionally, other actions can be restricted using the <code>ActionsGuarded</code> field on each <code>QualificationRequirement</code> structure. \"\n        }\n      ]\n    },\n    \"UniqueRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"<p> A unique identifier for this request which allows you to retry the call on error without creating duplicate HITs. This is useful in cases such as network timeouts where it is unclear whether or not the call succeeded on the server. If the HIT already exists in the\
  \ system from a previous call using the same UniqueRequestToken, subsequent calls will return a AWS.MechanicalTurk.HitAlreadyExists error with a message containing the HITId. </p> <note> <p> Note: It is your responsibility to ensure uniqueness of the token. The unique token expires after 24 hours. Subsequent calls using the same UniqueRequestToken made after the 24 hour limit could create duplicate HITs. </p> </note>\"\n        }\n      ]\n    },\n    \"AssignmentReviewPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewPolicy\"\n        },\n        {\n          \"description\": \" The Assignment-level Review Policy applies to the assignments under the HIT. You can specify for Mechanical Turk to take various actions based on the policy. \"\n        }\n      ]\n    },\n    \"HITReviewPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewPolicy\"\n        },\n        {\n          \"description\": \" The HIT-level\
  \ Review Policy applies to the HIT. You can specify for Mechanical Turk to take various actions based on the policy. \"\n        }\n      ]\n    },\n    \"HITLayoutId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"<p> The HITLayoutId allows you to use a pre-existing HIT design with placeholder values and create an additional HIT by providing those values as HITLayoutParameters. </p> <p> Constraints: Either a Question parameter or a HITLayoutId parameter must be provided. </p>\"\n        }\n      ]\n    },\n    \"HITLayoutParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HITLayoutParameterList\"\n        },\n        {\n          \"description\": \" If the HITLayoutId is provided, any placeholder values must be filled in with values using the HITLayoutParameter structure. For more information, see HITLayout. \"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"LifetimeInSeconds\",\n    \"AssignmentDurationInSeconds\",\n    \"Reward\",\n    \"Title\",\n    \"Description\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-hit-request-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: CreateHITRequest
---
