---
description: A code review in Perforce Helix Swarm (P4 Code Review), representing a set of changelists under review with participants, votes, state transitions, and test/deploy status.
layout: schema
name: Perforce Helix Swarm Review
properties_list:
- description: The unique review identifier assigned by Swarm.
  name: id
  type: integer
- description: The Perforce username of the review author.
  name: author
  type: string
- description: List of changelist IDs associated with this review.
  name: changes
  type: array
- description: List of committed changelist IDs resulting from this review.
  name: commits
  type: array
- description: Status details for commit operations on this review.
  name: commitStatus
  type: array
- description: Unix timestamp when the review was created.
  name: created
  type: integer
- description: Details of deployment operations triggered by this review.
  name: deployDetails
  type: array
- description: The current deployment status for the review.
  name: deployStatus
  type:
  - string
  - 'null'
- description: The review description, typically derived from the changelist description.
  name: description
  type: string
- description: Reviewer groups assigned to the review.
  name: groups
  type: array
- description: Map of participant usernames to their participation details, including votes and required status.
  name: participants
  type: object
- description: Whether the review is associated with a pending (shelved) changelist.
  name: pending
  type: boolean
- description: Map of Swarm project IDs to the branch names affected by this review.
  name: projects
  type: object
- description: Map of role names to lists of usernames holding those roles.
  name: roles
  type: object
- description: The current state of the review in its lifecycle.
  name: state
  type: string
- description: A human-readable label for the current state.
  name: stateLabel
  type: string
- description: Details of test runs executed against this review.
  name: testDetails
  type: array
- description: The overall test status for the review, such as pass or fail.
  name: testStatus
  type:
  - string
  - 'null'
- description: The review type. Default reviews are standard; personal reviews are private to the author.
  name: type
  type: string
- description: Unix timestamp when the review was last updated.
  name: updated
  type: integer
- description: ISO 8601 formatted date-time when the review was last updated.
  name: updateDate
  type: string
- description: History of review versions, each representing an update to the shelved changelist.
  name: versions
  type: array
provider_name: Perforce
provider_slug: perforce
schema_file: json-schema/perforce-review-schema.json
slug: perforce-review
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://perforce.com/schemas/swarm/review.json\",\n  \"title\": \"Perforce Helix Swarm Review\",\n  \"description\": \"A code review in Perforce Helix Swarm (P4 Code Review), representing a set of changelists under review with participants, votes, state transitions, and test/deploy status.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"author\", \"state\", \"description\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The unique review identifier assigned by Swarm.\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"The Perforce username of the review author.\"\n    },\n    \"changes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"minimum\": 1\n      },\n      \"description\": \"List of changelist IDs associated with this review.\"\n   \
  \ },\n    \"commits\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"minimum\": 1\n      },\n      \"description\": \"List of committed changelist IDs resulting from this review.\"\n    },\n    \"commitStatus\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CommitStatus\"\n      },\n      \"description\": \"Status details for commit operations on this review.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the review was created.\"\n    },\n    \"deployDetails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeployDetail\"\n      },\n      \"description\": \"Details of deployment operations triggered by this review.\"\n    },\n    \"deployStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The current deployment status for the review.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The review description, typically derived from the changelist description.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ReviewerGroup\"\n      },\n      \"description\": \"Reviewer groups assigned to the review.\"\n    },\n    \"participants\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Participant\"\n      },\n      \"description\": \"Map of participant usernames to their participation details, including votes and required status.\"\n    },\n    \"pending\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the review is associated with a pending (shelved) changelist.\"\n    },\n    \"projects\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Map of Swarm project IDs to the branch names\
  \ affected by this review.\"\n    },\n    \"roles\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Map of role names to lists of usernames holding those roles.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"needsReview\", \"needsRevision\", \"approved\", \"archived\", \"rejected\"],\n      \"description\": \"The current state of the review in its lifecycle.\"\n    },\n    \"stateLabel\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable label for the current state.\"\n    },\n    \"testDetails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TestDetail\"\n      },\n      \"description\": \"Details of test runs executed against this review.\"\n    },\n    \"testStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The overall test\
  \ status for the review, such as pass or fail.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"default\", \"personal\"],\n      \"description\": \"The review type. Default reviews are standard; personal reviews are private to the author.\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the review was last updated.\"\n    },\n    \"updateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 formatted date-time when the review was last updated.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ReviewVersion\"\n      },\n      \"description\": \"History of review versions, each representing an update to the shelved changelist.\"\n    }\n  },\n  \"$defs\": {\n    \"Participant\": {\n      \"type\": \"object\",\n      \"description\": \"A participant in a code review, including their vote and required\
  \ status.\",\n      \"properties\": {\n        \"vote\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"integer\",\n              \"enum\": [-1, 0, 1],\n              \"description\": \"The vote value: 1 for up, -1 for down, 0 for no vote.\"\n            },\n            \"version\": {\n              \"type\": \"integer\",\n              \"description\": \"The review version the vote was cast on.\"\n            },\n            \"isStale\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the vote is stale due to subsequent review updates.\"\n            }\n          },\n          \"description\": \"The participant's vote on the review.\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the participant is a required reviewer.\"\n        }\n      }\n    },\n    \"ReviewerGroup\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A group of reviewers assigned to a review.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the reviewer group.\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether at least one member of the group must approve the review.\"\n        },\n        \"quorum\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of group members required to approve. Zero means all members.\"\n        }\n      }\n    },\n    \"ReviewVersion\": {\n      \"type\": \"object\",\n      \"description\": \"A version snapshot of the review, created each time the shelved changelist is updated.\",\n      \"required\": [\"change\"],\n      \"properties\": {\n        \"difference\": {\n          \"type\": \"integer\",\n          \"description\": \"The difference type indicator.\"\n        },\n        \"stream\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The stream path, if applicable.\"\n        },\n        \"change\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The changelist number for this version.\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"The user who created this version.\"\n        },\n        \"time\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp when this version was created.\"\n        },\n        \"pending\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version represents a pending change.\"\n        },\n        \"archiveChange\": {\n          \"type\": \"integer\",\n          \"description\": \"The archive changelist number for this version.\"\n        }\n      }\n    },\n    \"CommitStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Status of a commit operation on the review.\",\n      \"properties\"\
  : {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The commit status value.\"\n        },\n        \"change\": {\n          \"type\": \"integer\",\n          \"description\": \"The associated changelist number.\"\n        },\n        \"committer\": {\n          \"type\": \"string\",\n          \"description\": \"The user who performed the commit.\"\n        },\n        \"start\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp when the commit was initiated.\"\n        },\n        \"end\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp when the commit completed.\"\n        }\n      }\n    },\n    \"DeployDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Details of a deployment triggered by the review.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The deployment status.\"\n        },\n        \"url\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the deployment details or environment.\"\n        },\n        \"error\": {\n          \"type\": \"string\",\n          \"description\": \"An error message if the deployment failed.\"\n        }\n      }\n    },\n    \"TestDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Details of a test run executed against the review.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The test run status.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the test run results.\"\n        },\n        \"error\": {\n          \"type\": \"string\",\n          \"description\": \"An error message if the test run failed.\"\n        }\n      }\n    },\n    \"Comment\": {\n      \"type\": \"object\",\n      \"description\": \"A comment on a review\
  \ or changelist in Helix Swarm.\",\n      \"required\": [\"id\", \"body\", \"user\", \"topic\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The unique comment identifier.\"\n        },\n        \"attachments\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          },\n          \"description\": \"File attachments on the comment.\"\n        },\n        \"body\": {\n          \"type\": \"string\",\n          \"description\": \"The comment body text.\"\n        },\n        \"context\": {\n          \"$ref\": \"#/$defs/CommentContext\"\n        },\n        \"edited\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Unix timestamp of the last edit, or null if not edited.\"\n        },\n        \"flags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"\
  description\": \"Flags applied to the comment.\"\n        },\n        \"likes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Usernames of users who liked the comment.\"\n        },\n        \"taskState\": {\n          \"type\": \"string\",\n          \"enum\": [\"comment\", \"open\", \"closed\", \"verified\"],\n          \"description\": \"The task state of the comment.\"\n        },\n        \"time\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp when the comment was created.\"\n        },\n        \"topic\": {\n          \"type\": \"string\",\n          \"description\": \"The topic the comment belongs to, such as reviews/1234.\"\n        },\n        \"updated\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp of the last update.\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"\
  The Perforce username of the comment author.\"\n        }\n      }\n    },\n    \"CommentContext\": {\n      \"type\": \"object\",\n      \"description\": \"Inline context for a file-level comment, specifying the file, line numbers, and surrounding content.\",\n      \"properties\": {\n        \"file\": {\n          \"type\": \"string\",\n          \"description\": \"The depot file path for the inline comment.\"\n        },\n        \"leftLine\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The left-side (original) line number.\"\n        },\n        \"rightLine\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The right-side (modified) line number.\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Adjacent source code content for context.\"\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"The review version this comment applies\
  \ to.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/json-schema/perforce-review-schema.json
tags: []
title: Perforce Helix Swarm Review
---
