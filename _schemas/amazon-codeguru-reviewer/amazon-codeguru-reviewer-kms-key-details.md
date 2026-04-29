---
description: <p>An object that contains:</p> <ul> <li> <p>The encryption option for a repository association. It is either owned by Amazon Web Services Key Management Service (KMS) (<code>AWS_OWNED_CMK</code>) or customer managed (<code>CUSTOMER_MANAGED_CMK</code>).</p> </li> <li> <p>The ID of the Amazon Web Services KMS key that is associated with a repository association.</p> </li> </ul>
layout: schema
name: KMSKeyDetails
properties_list:
- description: ''
  name: KMSKeyId
  type: object
- description: ''
  name: EncryptionOption
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-kms-key-details-schema.json
slug: amazon-codeguru-reviewer-kms-key-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-kms-key-details-schema.json\",\n  \"title\": \"KMSKeyDetails\",\n  \"description\": \"<p>An object that contains:</p> <ul> <li> <p>The encryption option for a repository association. It is either owned by Amazon Web Services Key Management Service (KMS) (<code>AWS_OWNED_CMK</code>) or customer managed (<code>CUSTOMER_MANAGED_CMK</code>).</p> </li> <li> <p>The ID of the Amazon Web Services KMS key that is associated with a repository association.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KMSKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KMSKeyId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services KMS key that is associated with a repository association.\"\n        }\n\
  \      ]\n    },\n    \"EncryptionOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionOption\"\n        },\n        {\n          \"description\": \"The encryption option for a repository association. It is either owned by Amazon Web Services Key Management Service (KMS) (<code>AWS_OWNED_CMK</code>) or customer managed (<code>CUSTOMER_MANAGED_CMK</code>).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-kms-key-details-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: KMSKeyDetails
---
