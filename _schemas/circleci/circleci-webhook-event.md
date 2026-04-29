---
description: Schema for CircleCI outbound webhook event payloads delivered via HTTP POST when workflow or job events occur in CI/CD pipelines.
layout: schema
name: CircleCI Webhook Event
properties_list:
- description: Unique identifier for the webhook delivery, used for deduplication
  name: id
  type: string
- description: The type of webhook event
  name: type
  type: string
- description: ISO 8601 timestamp of when the event occurred
  name: happened_at
  type: string
- description: ''
  name: webhook
  type: object
- description: ''
  name: project
  type: object
- description: ''
  name: organization
  type: object
- description: ''
  name: workflow
  type: object
- description: ''
  name: job
  type: object
- description: ''
  name: pipeline
  type: object
provider_name: CircleCI
provider_slug: circleci
schema_file: json-schema/circleci-webhook-event-schema.json
slug: circleci-webhook-event
source_filename: circleci-webhook-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://circleci.com/schemas/circleci/webhook-event.json\",\n  \"title\": \"CircleCI Webhook Event\",\n  \"description\": \"Schema for CircleCI outbound webhook event payloads delivered via HTTP POST when workflow or job events occur in CI/CD pipelines.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"happened_at\", \"webhook\", \"project\", \"organization\", \"pipeline\"],\n  \"discriminator\": {\n    \"propertyName\": \"type\"\n  },\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the webhook delivery, used for deduplication\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"workflow-completed\", \"job-completed\"],\n      \"description\": \"The type of webhook event\"\n    },\n    \"happened_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"ISO 8601 timestamp of when the event occurred\"\n    },\n    \"webhook\": {\n      \"$ref\": \"#/$defs/WebhookReference\"\n    },\n    \"project\": {\n      \"$ref\": \"#/$defs/ProjectReference\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/$defs/OrganizationReference\"\n    },\n    \"workflow\": {\n      \"$ref\": \"#/$defs/WorkflowReference\"\n    },\n    \"job\": {\n      \"$ref\": \"#/$defs/JobReference\"\n    },\n    \"pipeline\": {\n      \"$ref\": \"#/$defs/PipelineReference\"\n    }\n  },\n  \"$defs\": {\n    \"WebhookReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the webhook subscription that generated this delivery\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the webhook subscription\"\n        },\n        \"name\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The name of the webhook subscription\"\n        }\n      }\n    },\n    \"ProjectReference\": {\n      \"type\": \"object\",\n      \"description\": \"The project associated with the event\",\n      \"required\": [\"id\", \"name\", \"slug\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the project\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the project (repository name)\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"The project slug in vcs-type/org-name/repo-name format\",\n          \"pattern\": \"^[^/]+/[^/]+/[^/]+$\"\n        }\n      }\n    },\n    \"OrganizationReference\": {\n      \"type\": \"object\",\n      \"description\": \"The organization that owns the project\",\n      \"required\": [\"id\", \"name\"],\n  \
  \    \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the organization\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the organization\"\n        }\n      }\n    },\n    \"WorkflowReference\": {\n      \"type\": \"object\",\n      \"description\": \"The workflow associated with the event\",\n      \"required\": [\"id\", \"name\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the workflow\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the workflow\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the workflow was created\"\n      \
  \  },\n        \"stopped_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the workflow stopped\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to view the workflow in CircleCI\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"success\", \"failed\", \"error\", \"canceled\", \"unauthorized\"],\n          \"description\": \"The terminal status of the workflow\"\n        }\n      }\n    },\n    \"JobReference\": {\n      \"type\": \"object\",\n      \"description\": \"The job associated with the event (present only in job-completed events)\",\n      \"required\": [\"id\", \"name\", \"status\", \"number\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the job\"\n        },\n       \
  \ \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the job\"\n        },\n        \"number\": {\n          \"type\": \"integer\",\n          \"description\": \"The job number\"\n        },\n        \"started_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the job started\"\n        },\n        \"stopped_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the job stopped\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"success\", \"failed\", \"canceled\", \"infrastructure_fail\"],\n          \"description\": \"The terminal status of the job\"\n        }\n      }\n    },\n    \"PipelineReference\": {\n      \"type\": \"object\",\n      \"description\": \"The pipeline associated with the event\",\n      \"required\": [\"id\", \"number\", \"created_at\"],\n      \"properties\": {\n\
  \        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the pipeline\"\n        },\n        \"number\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The pipeline number\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the pipeline was created\"\n        },\n        \"trigger\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"The type of trigger that started the pipeline\"\n            }\n          },\n          \"description\": \"Trigger information\"\n        },\n        \"vcs\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"provider_name\": {\n              \"type\": \"string\",\n              \"description\": \"The\
  \ VCS provider name\"\n            },\n            \"origin_repository_url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The origin repository URL\"\n            },\n            \"target_repository_url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The target repository URL\"\n            },\n            \"revision\": {\n              \"type\": \"string\",\n              \"description\": \"The VCS revision (commit SHA)\"\n            },\n            \"branch\": {\n              \"type\": \"string\",\n              \"description\": \"The branch name\"\n            },\n            \"tag\": {\n              \"type\": \"string\",\n              \"description\": \"The tag name\"\n            },\n            \"commit\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"subject\": {\n                  \"type\": \"string\",\n\
  \                  \"description\": \"The commit message subject\"\n                },\n                \"body\": {\n                  \"type\": \"string\",\n                  \"description\": \"The commit message body\"\n                },\n                \"author\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": {\n                      \"type\": \"string\",\n                      \"description\": \"Author name\"\n                    },\n                    \"email\": {\n                      \"type\": \"string\",\n                      \"format\": \"email\",\n                      \"description\": \"Author email\"\n                    }\n                  },\n                  \"description\": \"Commit author\"\n                },\n                \"authored_at\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\",\n                  \"description\": \"When the commit was authored\"\
  \n                },\n                \"committer\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": {\n                      \"type\": \"string\",\n                      \"description\": \"Committer name\"\n                    },\n                    \"email\": {\n                      \"type\": \"string\",\n                      \"format\": \"email\",\n                      \"description\": \"Committer email\"\n                    }\n                  },\n                  \"description\": \"Commit committer\"\n                },\n                \"committed_at\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\",\n                  \"description\": \"When the commit was committed\"\n                }\n              },\n              \"description\": \"Commit details\"\n            }\n          },\n          \"description\": \"VCS information\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/json-schema/circleci-webhook-event-schema.json
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
title: CircleCI Webhook Event
---
