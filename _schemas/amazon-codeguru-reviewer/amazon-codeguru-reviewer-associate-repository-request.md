---
description: AssociateRepositoryRequest schema from Amazon CodeGuru Reviewer
layout: schema
name: AssociateRepositoryRequest
properties_list:
- description: ''
  name: Repository
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: KMSKeyDetails
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-associate-repository-request-schema.json
slug: amazon-codeguru-reviewer-associate-repository-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-associate-repository-request-schema.json\",\n  \"title\": \"AssociateRepositoryRequest\",\n  \"description\": \"AssociateRepositoryRequest schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Repository\"\n        },\n        {\n          \"description\": \"The repository to associate.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Amazon CodeGuru Reviewer uses this value to prevent the accidental creation of duplicate repository associations if there are failures and retries.\"\n\
  \        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>An array of key-value pairs used to tag an associated repository. A tag is a custom attribute label with two parts:</p> <ul> <li> <p>A <i>tag key</i> (for example, <code>CostCenter</code>, <code>Environment</code>, <code>Project</code>, or <code>Secret</code>). Tag keys are case sensitive.</p> </li> <li> <p>An optional field known as a <i>tag value</i> (for example, <code>111122223333</code>, <code>Production</code>, or a team name). Omitting the tag value is the same as using an empty string. Like tag keys, tag values are case sensitive.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"KMSKeyDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KMSKeyDetails\"\n        },\n        {\n          \"description\": \"<p>A <code>KMSKeyDetails</code> object that contains:</p>\
  \ <ul> <li> <p>The encryption option for this repository association. It is either owned by Amazon Web Services Key Management Service (KMS) (<code>AWS_OWNED_CMK</code>) or customer managed (<code>CUSTOMER_MANAGED_CMK</code>).</p> </li> <li> <p>The ID of the Amazon Web Services KMS key that is associated with this repository association.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Repository\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-associate-repository-request-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: AssociateRepositoryRequest
---
