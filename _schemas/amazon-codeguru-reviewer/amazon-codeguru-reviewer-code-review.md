---
description: Information about a code review. A code review belongs to the associated repository that contains the reviewed code.
layout: schema
name: CodeReview
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: CodeReviewArn
  type: object
- description: ''
  name: RepositoryName
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: ProviderType
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: StateReason
  type: object
- description: ''
  name: CreatedTimeStamp
  type: object
- description: ''
  name: LastUpdatedTimeStamp
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: PullRequestId
  type: object
- description: ''
  name: SourceCodeType
  type: object
- description: ''
  name: AssociationArn
  type: object
- description: ''
  name: Metrics
  type: object
- description: ''
  name: AnalysisTypes
  type: object
- description: ''
  name: ConfigFileState
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-code-review-schema.json
slug: amazon-codeguru-reviewer-code-review
source_filename: amazon-codeguru-reviewer-code-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-review-schema.json\",\n  \"title\": \"CodeReview\",\n  \"description\": \"Information about a code review. A code review belongs to the associated repository that contains the reviewed code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the code review.\"\n        }\n      ]\n    },\n    \"CodeReviewArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CodeReview.html\\\">CodeReview</a> object. \"\n    \
  \    }\n      ]\n    },\n    \"RepositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the repository.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Owner\"\n        },\n        {\n          \"description\": \"The owner of the repository. For an Amazon Web Services CodeCommit repository, this is the Amazon Web Services account ID of the account that owns the repository. For a GitHub, GitHub Enterprise Server, or Bitbucket repository, this is the username for the account that owns the repository. For an S3 repository, it can be the username or Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"ProviderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderType\"\n        },\n        {\n          \"description\": \"The type of repository that contains\
  \ the reviewed code (for example, GitHub or Bitbucket).\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobState\"\n        },\n        {\n          \"description\": \"<p>The valid code review states are:</p> <ul> <li> <p> <code>Completed</code>: The code review is complete.</p> </li> <li> <p> <code>Pending</code>: The code review started and has not completed or failed.</p> </li> <li> <p> <code>Failed</code>: The code review failed.</p> </li> <li> <p> <code>Deleting</code>: The code review is being deleted.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"StateReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateReason\"\n        },\n        {\n          \"description\": \"The reason for the state of the code review.\"\n        }\n      ]\n    },\n    \"CreatedTimeStamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n      \
  \  },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the code review was created.\"\n        }\n      ]\n    },\n    \"LastUpdatedTimeStamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the code review was last updated.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"description\": \"The type of code review.\"\n        }\n      ]\n    },\n    \"PullRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PullRequestId\"\n        },\n        {\n          \"description\": \"The pull request ID for the code review.\"\n        }\n      ]\n    },\n    \"SourceCodeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceCodeType\"\
  \n        },\n        {\n          \"description\": \"The type of the source code for the code review.\"\n        }\n      ]\n    },\n    \"AssociationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociationArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociation.html\\\">RepositoryAssociation</a> that contains the reviewed source code. You can retrieve associated repository ARNs by calling <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_ListRepositoryAssociations.html\\\">ListRepositoryAssociations</a>.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metrics\"\n        },\n        {\n          \"description\": \"The statistics from the code review.\"\n        }\n      ]\n    },\n    \"AnalysisTypes\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalysisTypes\"\n        },\n        {\n          \"description\": \"The types of analysis performed during a repository analysis or a pull request review. You can specify either <code>Security</code>, <code>CodeQuality</code>, or both.\"\n        }\n      ]\n    },\n    \"ConfigFileState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigFileState\"\n        },\n        {\n          \"description\": \"The state of the <code>aws-codeguru-reviewer.yml</code> configuration file that allows the configuration of the CodeGuru Reviewer analysis. The file either exists, doesn't exist, or exists with errors at the root directory of your repository.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-review-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: CodeReview
---
