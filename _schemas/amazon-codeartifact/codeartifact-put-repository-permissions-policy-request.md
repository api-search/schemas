---
description: PutRepositoryPermissionsPolicyRequest schema from Amazon CodeArtifact API
layout: schema
name: PutRepositoryPermissionsPolicyRequest
properties_list:
- description: ''
  name: policyRevision
  type: object
- description: ''
  name: policyDocument
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-put-repository-permissions-policy-request-schema.json
slug: codeartifact-put-repository-permissions-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-repository-permissions-policy-request-schema.json\",\n  \"title\": \"PutRepositoryPermissionsPolicyRequest\",\n  \"description\": \"PutRepositoryPermissionsPolicyRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevision\"\n        },\n        {\n          \"description\": \" Sets the revision of the resource policy that specifies permissions to access the repository. This revision is used for optimistic locking, which prevents others from overwriting your changes to the repository's resource policy. \"\n        }\n      ]\n    },\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\
  \n        },\n        {\n          \"description\": \" A valid displayable JSON Aspen policy string to be set as the access control resource policy on the provided repository. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policyDocument\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-repository-permissions-policy-request-schema.json
tags:
- Amazon
- AWS
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: PutRepositoryPermissionsPolicyRequest
---
