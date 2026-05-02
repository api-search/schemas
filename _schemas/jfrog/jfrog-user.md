---
description: Represents a user account in the JFrog Platform, managed by the Access service for authentication and authorization across all JFrog services.
layout: schema
name: JFrog Platform User
properties_list:
- description: Unique username identifying the user across the platform
  name: username
  type: string
- description: User email address
  name: email
  type: string
- description: Whether the user has platform administrator privileges
  name: admin
  type: boolean
- description: Whether the user can update their own profile information
  name: profile_updatable
  type: boolean
- description: Whether browser-based UI access is disabled for this user
  name: disable_ui_access
  type: boolean
- description: Whether internal password authentication is disabled (forces external auth)
  name: internal_password_disabled
  type: boolean
- description: User account status
  name: status
  type: string
- description: Groups the user belongs to
  name: groups
  type: array
- description: Authentication realm indicating the identity provider
  name: realm
  type: string
- description: Timestamp of the user's last login
  name: last_logged_in
  type: string
- description: Timestamp when the user account was created
  name: created
  type: string
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-user-schema.json
slug: jfrog-user
source_filename: jfrog-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/user\",\n  \"title\": \"JFrog Platform User\",\n  \"description\": \"Represents a user account in the JFrog Platform, managed by the Access service for authentication and authorization across all JFrog services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Unique username identifying the user across the platform\",\n      \"examples\": [\n        \"admin\",\n        \"developer1\"\n      ]\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address\"\n    },\n    \"admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has platform administrator privileges\",\n      \"default\": false\n    },\n    \"profile_updatable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user\
  \ can update their own profile information\",\n      \"default\": true\n    },\n    \"disable_ui_access\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether browser-based UI access is disabled for this user\",\n      \"default\": false\n    },\n    \"internal_password_disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether internal password authentication is disabled (forces external auth)\",\n      \"default\": false\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"User account status\",\n      \"enum\": [\n        \"enabled\",\n        \"disabled\"\n      ]\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Groups the user belongs to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"realm\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication realm indicating the identity provider\",\n      \"enum\": [\n        \"internal\",\n        \"ldap\"\
  ,\n        \"saml\",\n        \"oauth\",\n        \"crowd\"\n      ]\n    },\n    \"last_logged_in\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the user's last login\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user account was created\"\n    }\n  },\n  \"required\": [\n    \"username\",\n    \"email\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-user-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Platform User
---
