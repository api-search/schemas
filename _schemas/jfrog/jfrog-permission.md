---
description: Represents a permission target in the JFrog Platform, defining access control rules for repositories, builds, and release bundles. Permissions control which users and groups can perform specific actions on specific resources.
layout: schema
name: JFrog Permission Target
properties_list:
- description: Unique name identifying the permission target
  name: name
  type: string
- description: Resource-level access control definitions
  name: resources
  type: object
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-permission-schema.json
slug: jfrog-permission
source_filename: jfrog-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/permission\",\n  \"title\": \"JFrog Permission Target\",\n  \"description\": \"Represents a permission target in the JFrog Platform, defining access control rules for repositories, builds, and release bundles. Permissions control which users and groups can perform specific actions on specific resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name identifying the permission target\",\n      \"examples\": [\n        \"release-deployers\",\n        \"dev-team-readers\"\n      ]\n    },\n    \"resources\": {\n      \"type\": \"object\",\n      \"description\": \"Resource-level access control definitions\",\n      \"properties\": {\n        \"repository\": {\n          \"type\": \"object\",\n          \"description\": \"Repository-level permissions keyed by repository name\",\n       \
  \   \"additionalProperties\": {\n            \"$ref\": \"#/$defs/ResourcePermission\"\n          }\n        },\n        \"build\": {\n          \"type\": \"object\",\n          \"description\": \"Build-level permissions keyed by build pattern\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/ResourcePermission\"\n          }\n        },\n        \"releaseBundle\": {\n          \"type\": \"object\",\n          \"description\": \"Release bundle-level permissions\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/ResourcePermission\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"$defs\": {\n    \"ResourcePermission\": {\n      \"type\": \"object\",\n      \"description\": \"Permission rules for a specific resource\",\n      \"properties\": {\n        \"include_patterns\": {\n          \"type\": \"array\",\n          \"description\": \"Patterns for included paths (Ant-style)\",\n          \"items\"\
  : {\n            \"type\": \"string\"\n          },\n          \"default\": [\"**\"]\n        },\n        \"exclude_patterns\": {\n          \"type\": \"array\",\n          \"description\": \"Patterns for excluded paths\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"default\": []\n        },\n        \"actions\": {\n          \"type\": \"object\",\n          \"description\": \"Action grants for users and groups\",\n          \"properties\": {\n            \"users\": {\n              \"type\": \"object\",\n              \"description\": \"User-specific action grants (username -> actions array)\",\n              \"additionalProperties\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"read\",\n                    \"write\",\n                    \"annotate\",\n                    \"delete\",\n                    \"manage\",\n       \
  \             \"managedXrayMeta\",\n                    \"distribute\"\n                  ]\n                }\n              }\n            },\n            \"groups\": {\n              \"type\": \"object\",\n              \"description\": \"Group-specific action grants (group name -> actions array)\",\n              \"additionalProperties\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"read\",\n                    \"write\",\n                    \"annotate\",\n                    \"delete\",\n                    \"manage\",\n                    \"managedXrayMeta\",\n                    \"distribute\"\n                  ]\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-permission-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Permission Target
---
