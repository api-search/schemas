---
description: Properties of user.
layout: schema
name: User
properties_list:
- description: User name
  name: name
  type: string
- description: Password
  name: password
  type: string
- description: Login name
  name: login_name
  type: string
- description: Display name
  name: display_name
  type: string
- description: First name
  name: first_name
  type: string
- description: Middle name
  name: middle_name
  type: string
- description: Last name
  name: last_name
  type: string
- description: Email address
  name: email
  type: string
- description: Does this user need to change their password (e.g., after assigning a temp password)
  name: must_change_password
  type: boolean
- description: Has this user been disabled from the system
  name: disabled
  type: boolean
- description: How many days until this user expires
  name: days_to_expiry
  type: integer
- description: How many minutes until the account is unlocked after multiple failed logins
  name: mins_to_unlock
  type: integer
- description: The default warehouse to use when this user starts a session
  name: default_warehouse
  type: string
- description: The default namespace to use when this user starts a session
  name: default_namespace
  type: string
- description: The default role to use when this user starts a session
  name: default_role
  type: string
- description: The default secondary roles of this user to use when starting a session. Only valid set values are ALL or NONE. Default is ALL after 2024-07 BCR.
  name: default_secondary_roles
  type: string
- description: How many minutes until MFA is required again
  name: mins_to_bypass_mfa
  type: integer
- description: RSA public key of the user
  name: rsa_public_key
  type: string
- description: Second RSA public key of the user
  name: rsa_public_key_2
  type: string
- description: Comment about the user.
  name: comment
  type: string
- description: Indicates the type of user (PERSON | SERVICE | LEGACY_SERVICE)
  name: type
  type: string
- description: Whether to show unredacted query syntax errors in the query history.
  name: enable_unredacted_query_syntax_error
  type: boolean
- description: Specifies an existing network policy is active for the user. Otherwise, use account default.
  name: network_policy
  type: string
- description: ''
  name: created_on
  type: string
- description: ''
  name: last_successful_login
  type: string
- description: ''
  name: expires_at
  type: string
- description: ''
  name: locked_until
  type: string
- description: ''
  name: has_password
  type: boolean
- description: ''
  name: has_rsa_public_key
  type: boolean
- description: Fingerprint of the user's RSA public key
  name: rsa_public_key_fp
  type: string
- description: Fingerprint of the user's second RSA public key
  name: rsa_public_key_2_fp
  type: string
- description: ''
  name: ext_authn_duo
  type: boolean
- description: ''
  name: ext_authn_uid
  type: string
- description: ''
  name: owner
  type: string
- description: Whether the user, account, or organization is locked by Snowflake.
  name: snowflake_lock
  type: boolean
- description: Whether Snowflake Support is allowed to use the user or account
  name: snowflake_support
  type: boolean
- description: Temporary bypass network policy on the user for a specified number of minutes
  name: mins_to_bypass_network_policy
  type: integer
- description: ''
  name: password_last_set
  type: string
- description: ''
  name: custom_landing_page_url
  type: string
- description: Whether or not to flush the custom landing page of the user on next UI load
  name: custom_landing_page_url_flush_next_ui_load
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-user-schema.json
slug: user-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"Properties of user.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User name\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password\"\n    },\n    \"login_name\": {\n      \"type\": \"string\",\n      \"description\": \"Login name\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"middle_name\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    },\n    \"must_change_password\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Does this user need to change their password (e.g., after assigning a temp password)\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has this user been disabled from the system\"\n    },\n    \"days_to_expiry\": {\n      \"type\": \"integer\",\n      \"description\": \"How many days until this user expires\"\n    },\n    \"mins_to_unlock\": {\n      \"type\": \"integer\",\n      \"description\": \"How many minutes until the account is unlocked after multiple failed logins\"\n    },\n    \"default_warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"The default warehouse to use when this user starts a session\"\n    },\n    \"default_namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The default namespace to use when this user starts a session\"\n    },\n    \"default_role\": {\n      \"type\": \"string\",\n      \"description\": \"The default role to use\
  \ when this user starts a session\"\n    },\n    \"default_secondary_roles\": {\n      \"type\": \"string\",\n      \"description\": \"The default secondary roles of this user to use when starting a session. Only valid set values are ALL or NONE. Default is ALL after 2024-07 BCR.\"\n    },\n    \"mins_to_bypass_mfa\": {\n      \"type\": \"integer\",\n      \"description\": \"How many minutes until MFA is required again\"\n    },\n    \"rsa_public_key\": {\n      \"type\": \"string\",\n      \"description\": \"RSA public key of the user\"\n    },\n    \"rsa_public_key_2\": {\n      \"type\": \"string\",\n      \"description\": \"Second RSA public key of the user\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment about the user.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the type of user (PERSON | SERVICE | LEGACY_SERVICE)\"\n    },\n    \"enable_unredacted_query_syntax_error\": {\n      \"type\":\
  \ \"boolean\",\n      \"description\": \"Whether to show unredacted query syntax errors in the query history.\"\n    },\n    \"network_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies an existing network policy is active for the user. Otherwise, use account default.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\"\n    },\n    \"last_successful_login\": {\n      \"type\": \"string\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\"\n    },\n    \"locked_until\": {\n      \"type\": \"string\"\n    },\n    \"has_password\": {\n      \"type\": \"boolean\"\n    },\n    \"has_rsa_public_key\": {\n      \"type\": \"boolean\"\n    },\n    \"rsa_public_key_fp\": {\n      \"type\": \"string\",\n      \"description\": \"Fingerprint of the user's RSA public key\"\n    },\n    \"rsa_public_key_2_fp\": {\n      \"type\": \"string\",\n      \"description\": \"Fingerprint of the user's second RSA public key\"\n    },\n    \"ext_authn_duo\": {\n      \"\
  type\": \"boolean\"\n    },\n    \"ext_authn_uid\": {\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"type\": \"string\"\n    },\n    \"snowflake_lock\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user, account, or organization is locked by Snowflake.\"\n    },\n    \"snowflake_support\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Snowflake Support is allowed to use the user or account\"\n    },\n    \"mins_to_bypass_network_policy\": {\n      \"type\": \"integer\",\n      \"description\": \"Temporary bypass network policy on the user for a specified number of minutes\"\n    },\n    \"password_last_set\": {\n      \"type\": \"string\"\n    },\n    \"custom_landing_page_url\": {\n      \"type\": \"string\"\n    },\n    \"custom_landing_page_url_flush_next_ui_load\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether or not to flush the custom landing page of the user on next UI load\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-user-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: User
---
