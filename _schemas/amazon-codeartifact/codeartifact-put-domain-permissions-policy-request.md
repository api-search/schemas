---
description: PutDomainPermissionsPolicyRequest schema from Amazon CodeArtifact API
layout: schema
name: PutDomainPermissionsPolicyRequest
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: domainOwner
  type: object
- description: ''
  name: policyRevision
  type: object
- description: ''
  name: policyDocument
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-put-domain-permissions-policy-request-schema.json
slug: codeartifact-put-domain-permissions-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-domain-permissions-policy-request-schema.json\",\n  \"title\": \"PutDomainPermissionsPolicyRequest\",\n  \"description\": \"PutDomainPermissionsPolicyRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \" The name of the domain on which to set the resource policy. \"\n        }\n      ]\n    },\n    \"domainOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \" The 12-digit account number of the Amazon Web Services account that owns the domain. It does not include dashes or spaces. \"\n    \
  \    }\n      ]\n    },\n    \"policyRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRevision\"\n        },\n        {\n          \"description\": \" The current revision of the resource policy to be set. This revision is used for optimistic locking, which prevents others from overwriting your changes to the domain's resource policy. \"\n        }\n      ]\n    },\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \" A valid displayable JSON Aspen policy string to be set as the access control resource policy on the provided domain. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"domain\",\n    \"policyDocument\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-domain-permissions-policy-request-schema.json
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
title: PutDomainPermissionsPolicyRequest
---
