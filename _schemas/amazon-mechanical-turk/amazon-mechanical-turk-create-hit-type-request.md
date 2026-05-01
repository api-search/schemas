---
description: CreateHITTypeRequest schema from Amazon Mechanical Turk API
layout: schema
name: CreateHITTypeRequest
properties_list:
- description: ''
  name: AutoApprovalDelayInSeconds
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
  name: QualificationRequirements
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-create-hit-type-request-schema.json
slug: amazon-mechanical-turk-create-hit-type-request
source_filename: amazon-mechanical-turk-create-hit-type-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-hit-type-request-schema.json\",\n  \"title\": \"CreateHITTypeRequest\",\n  \"description\": \"CreateHITTypeRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoApprovalDelayInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The number of seconds after an assignment for the HIT has been submitted, after which the assignment is considered Approved automatically unless the Requester explicitly rejects it. \"\n        }\n      ]\n    },\n    \"AssignmentDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The amount\
  \ of time, in seconds, that a Worker has to complete the HIT after accepting it. If a Worker does not complete the assignment within the specified duration, the assignment is considered abandoned. If the HIT is still active (that is, its lifetime has not elapsed), the assignment becomes available for other users to find and accept. \"\n        }\n      ]\n    },\n    \"Reward\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrencyAmount\"\n        },\n        {\n          \"description\": \" The amount of money the Requester will pay a Worker for successfully completing the HIT. \"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The title of the HIT. A title should be short and descriptive about the kind of task the HIT contains. On the Amazon Mechanical Turk web site, the HIT title appears in search results, and everywhere\
  \ the HIT is mentioned. \"\n        }\n      ]\n    },\n    \"Keywords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" One or more words or phrases that describe the HIT, separated by commas. These words are used in searches to find HITs. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A general description of the HIT. A description includes detailed information about the kind of task the HIT contains. On the Amazon Mechanical Turk web site, the HIT description appears in the expanded view of search results, and in the HIT and assignment screens. A good description gives the user enough information to evaluate the HIT before accepting it. \"\n        }\n      ]\n    },\n    \"QualificationRequirements\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/QualificationRequirementList\"\n        },\n        {\n          \"description\": \" Conditions that a Worker's Qualifications must meet in order to accept the HIT. A HIT can have between zero and ten Qualification requirements. All requirements must be met in order for a Worker to accept the HIT. Additionally, other actions can be restricted using the <code>ActionsGuarded</code> field on each <code>QualificationRequirement</code> structure. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AssignmentDurationInSeconds\",\n    \"Reward\",\n    \"Title\",\n    \"Description\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-hit-type-request-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: CreateHITTypeRequest
---
