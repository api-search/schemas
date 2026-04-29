---
description: A code review in Helix Swarm, representing a set of changes under review with participants, votes, and state.
layout: schema
name: Review
properties_list:
- description: The unique review identifier.
  name: id
  type: integer
- description: The username of the review author.
  name: author
  type: string
- description: List of changelist IDs associated with the review.
  name: changes
  type: array
- description: List of committed changelist IDs.
  name: commits
  type: array
- description: Status of commit operations.
  name: commitStatus
  type: array
- description: Unix timestamp when the review was created.
  name: created
  type: integer
- description: Deploy configuration details.
  name: deployDetails
  type: array
- description: The current deploy status.
  name: deployStatus
  type: string
- description: The review description.
  name: description
  type: string
- description: Reviewer groups assigned to the review.
  name: groups
  type: array
- description: Map of participant usernames to their participation details including votes and required status.
  name: participants
  type: object
- description: Whether the review has a pending changelist.
  name: pending
  type: boolean
- description: Map of project IDs to affected branch names.
  name: projects
  type: object
- description: Map of roles to lists of usernames.
  name: roles
  type: object
- description: The current state of the review.
  name: state
  type: string
- description: A display-friendly label for the current state.
  name: stateLabel
  type: string
- description: Details of test runs.
  name: testDetails
  type: array
- description: The overall test status.
  name: testStatus
  type: string
- description: The review type (default or personal).
  name: type
  type: string
- description: Unix timestamp when the review was last updated.
  name: updated
  type: integer
- description: ISO 8601 formatted date when the review was last updated.
  name: updateDate
  type: string
- description: List of review version objects.
  name: versions
  type: array
provider_name: Perforce
provider_slug: perforce
schema_file: json-schema/perforce-helix-swarm-review-schema.json
slug: perforce-helix-swarm-review
source_filename: perforce-helix-swarm-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Review\",\n  \"type\": \"object\",\n  \"description\": \"A code review in Helix Swarm, representing a set of changes under review with participants, votes, and state.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique review identifier.\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the review author.\"\n    },\n    \"changes\": {\n      \"type\": \"array\",\n      \"description\": \"List of changelist IDs associated with the review.\"\n    },\n    \"commits\": {\n      \"type\": \"array\",\n      \"description\": \"List of committed changelist IDs.\"\n    },\n    \"commitStatus\": {\n      \"type\": \"array\",\n      \"description\": \"Status of commit operations.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the review was created.\"\
  \n    },\n    \"deployDetails\": {\n      \"type\": \"array\",\n      \"description\": \"Deploy configuration details.\"\n    },\n    \"deployStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current deploy status.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The review description.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Reviewer groups assigned to the review.\"\n    },\n    \"participants\": {\n      \"type\": \"object\",\n      \"description\": \"Map of participant usernames to their participation details including votes and required status.\"\n    },\n    \"pending\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the review has a pending changelist.\"\n    },\n    \"projects\": {\n      \"type\": \"object\",\n      \"description\": \"Map of project IDs to affected branch names.\"\n    },\n    \"roles\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Map of roles to lists of usernames.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the review.\"\n    },\n    \"stateLabel\": {\n      \"type\": \"string\",\n      \"description\": \"A display-friendly label for the current state.\"\n    },\n    \"testDetails\": {\n      \"type\": \"array\",\n      \"description\": \"Details of test runs.\"\n    },\n    \"testStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The overall test status.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The review type (default or personal).\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the review was last updated.\"\n    },\n    \"updateDate\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 formatted date when the review was last updated.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\":\
  \ \"List of review version objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/json-schema/perforce-helix-swarm-review-schema.json
tags: []
title: Review
---
