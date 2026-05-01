---
description: A directory entry accessed via the ForgeRock Directory Services HDAP (HTTP Directory Access Protocol) API. Represents an LDAP entry mapped to a JSON resource with standard person and organizational attributes.
layout: schema
name: ForgeRock Directory Entry
properties_list:
- description: Entry identifier mapped from the LDAP RDN attribute (e.g., uid)
  name: _id
  type: string
- description: Entry revision for MVCC concurrency control (mapped from LDAP etag)
  name: _rev
  type: string
- description: Login username (mapped from LDAP uid)
  name: userName
  type: string
- description: Common name (typically full name)
  name: cn
  type: string
- description: First name
  name: givenName
  type: string
- description: Surname / last name
  name: sn
  type: string
- description: Email address
  name: mail
  type: string
- description: Telephone number
  name: telephoneNumber
  type: string
- description: Entry description
  name: description
  type: string
- description: DNs of groups this entry belongs to (virtual attribute)
  name: memberOf
  type: array
- description: User password (write-only, stored as a hash in the directory)
  name: userPassword
  type: string
- description: Whether the account is disabled by password policy
  name: ds-pwp-account-disabled
  type: boolean
- description: Last successful authentication time
  name: ds-pwp-last-login-time
  type: string
- description: Entry creation time
  name: createTimestamp
  type: string
- description: Last modification time
  name: modifyTimestamp
  type: string
provider_name: ForgeRock
provider_slug: forgerock
schema_file: json-schema/forgerock-directory-entry-schema.json
slug: forgerock-directory-entry
source_filename: forgerock-directory-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.forgerock.com/directory-entry\",\n  \"title\": \"ForgeRock Directory Entry\",\n  \"description\": \"A directory entry accessed via the ForgeRock Directory Services HDAP (HTTP Directory Access Protocol) API. Represents an LDAP entry mapped to a JSON resource with standard person and organizational attributes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Entry identifier mapped from the LDAP RDN attribute (e.g., uid)\"\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Entry revision for MVCC concurrency control (mapped from LDAP etag)\",\n      \"readOnly\": true\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Login username (mapped from LDAP uid)\"\n    },\n    \"cn\": {\n      \"type\": \"string\",\n      \"description\": \"Common name (typically\
  \ full name)\"\n    },\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"sn\": {\n      \"type\": \"string\",\n      \"description\": \"Surname / last name\"\n    },\n    \"mail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address\"\n    },\n    \"telephoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Telephone number\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Entry description\"\n    },\n    \"memberOf\": {\n      \"type\": \"array\",\n      \"description\": \"DNs of groups this entry belongs to (virtual attribute)\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"userPassword\": {\n      \"type\": \"string\",\n      \"description\": \"User password (write-only, stored as a hash in the directory)\",\n      \"writeOnly\": true\n    },\n    \"ds-pwp-account-disabled\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account is disabled by password policy\"\n    },\n    \"ds-pwp-last-login-time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last successful authentication time\",\n      \"readOnly\": true\n    },\n    \"createTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Entry creation time\",\n      \"readOnly\": true\n    },\n    \"modifyTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"_id\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/json-schema/forgerock-directory-entry-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
title: ForgeRock Directory Entry
---
