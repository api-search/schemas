---
description: Summary information about a repository association. The <a href="https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_ListRepositoryAssociations.html">ListRepositoryAssociations</a> operation returns a list of <code>RepositoryAssociationSummary</code> objects.
layout: schema
name: RepositoryAssociationSummary
properties_list:
- description: ''
  name: AssociationArn
  type: object
- description: ''
  name: ConnectionArn
  type: object
- description: ''
  name: LastUpdatedTimeStamp
  type: object
- description: ''
  name: AssociationId
  type: object
- description: ''
  name: Name
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
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-repository-association-summary-schema.json
slug: amazon-codeguru-reviewer-repository-association-summary
source_filename: amazon-codeguru-reviewer-repository-association-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-association-summary-schema.json\",\n  \"title\": \"RepositoryAssociationSummary\",\n  \"description\": \"Summary information about a repository association. The <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_ListRepositoryAssociations.html\\\">ListRepositoryAssociations</a> operation returns a list of <code>RepositoryAssociationSummary</code> objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssociationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociation.html\\\">RepositoryAssociation</a> object. You\
  \ can retrieve this ARN by calling <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_ListRepositoryAssociations.html\\\">ListRepositoryAssociations</a>.\"\n        }\n      ]\n    },\n    \"ConnectionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an Amazon Web Services CodeStar Connections connection. Its format is <code>arn:aws:codestar-connections:region-id:aws-account_id:connection/connection-id</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/codestar-connections/latest/APIReference/API_Connection.html\\\">Connection</a> in the <i>Amazon Web Services CodeStar Connections API Reference</i>.\"\n        }\n      ]\n    },\n    \"LastUpdatedTimeStamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"The time,\
  \ in milliseconds since the epoch, since the repository association was last updated.\"\n        }\n      ]\n    },\n    \"AssociationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociationId\"\n        },\n        {\n          \"description\": \"The repository association ID.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the repository association.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Owner\"\n        },\n        {\n          \"description\": \"The owner of the repository. For an Amazon Web Services CodeCommit repository, this is the Amazon Web Services account ID of the account that owns the repository. For a GitHub, GitHub Enterprise Server, or Bitbucket repository, this is the username for the account that owns the\
  \ repository. For an S3 repository, it can be the username or Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"ProviderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderType\"\n        },\n        {\n          \"description\": \"The provider type of the repository association.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryAssociationState\"\n        },\n        {\n          \"description\": \"<p>The state of the repository association.</p> <p>The valid repository association states are:</p> <ul> <li> <p> <b>Associated</b>: The repository association is complete.</p> </li> <li> <p> <b>Associating</b>: CodeGuru Reviewer is:</p> <ul> <li> <p>Setting up pull request notifications. This is required for pull requests to trigger a CodeGuru Reviewer review.</p> <note> <p>If your repository <code>ProviderType</code> is <code>GitHub</code>, <code>GitHub\
  \ Enterprise Server</code>, or <code>Bitbucket</code>, CodeGuru Reviewer creates webhooks in your repository to trigger CodeGuru Reviewer reviews. If you delete these webhooks, reviews of code in your repository cannot be triggered.</p> </note> </li> <li> <p>Setting up source code access. This is required for CodeGuru Reviewer to securely clone code in your repository.</p> </li> </ul> </li> <li> <p> <b>Failed</b>: The repository failed to associate or disassociate.</p> </li> <li> <p> <b>Disassociating</b>: CodeGuru Reviewer is removing the repository's pull request notifications and source code access.</p> </li> <li> <p> <b>Disassociated</b>: CodeGuru Reviewer successfully disassociated the repository. You can create a new association with this repository if you want to review source code in it later. You can control access to code reviews created in anassociated repository with tags after it has been disassociated. For more information, see <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-ug/auth-and-access-control-using-tags.html\\\
  \">Using tags to control access to associated repositories</a> in the <i>Amazon CodeGuru Reviewer User Guide</i>.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-association-summary-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: RepositoryAssociationSummary
---
