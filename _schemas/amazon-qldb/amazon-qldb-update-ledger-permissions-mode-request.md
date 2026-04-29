---
description: UpdateLedgerPermissionsModeRequest schema from Amazon QLDB API
layout: schema
name: UpdateLedgerPermissionsModeRequest
properties_list:
- description: ''
  name: PermissionsMode
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-update-ledger-permissions-mode-request-schema.json
slug: amazon-qldb-update-ledger-permissions-mode-request
source_filename: amazon-qldb-update-ledger-permissions-mode-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-update-ledger-permissions-mode-request-schema.json\",\n  \"title\": \"UpdateLedgerPermissionsModeRequest\",\n  \"description\": \"UpdateLedgerPermissionsModeRequest schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PermissionsMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionsMode\"\n        },\n        {\n          \"description\": \"<p>The permissions mode to assign to the ledger. This parameter can have one of the following values:</p> <ul> <li> <p> <code>ALLOW_ALL</code>: A legacy permissions mode that enables access control with API-level granularity for ledgers.</p> <p>This mode allows users who have the <code>SendCommand</code> API permission for this ledger to run all PartiQL commands (hence, <code>ALLOW_ALL</code>)\
  \ on any tables in the specified ledger. This mode disregards any table-level or command-level IAM permissions policies that you create for the ledger.</p> </li> <li> <p> <code>STANDARD</code>: (<i>Recommended</i>) A permissions mode that enables access control with finer granularity for ledgers, tables, and PartiQL commands.</p> <p>By default, this mode denies all user requests to run any PartiQL commands on any tables in this ledger. To allow PartiQL commands to run, you must create IAM permissions policies for specific table resources and PartiQL actions, in addition to the <code>SendCommand</code> API permission for the ledger. For information, see <a href=\\\"https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started-standard-mode.html\\\">Getting started with the standard permissions mode</a> in the <i>Amazon QLDB Developer Guide</i>.</p> </li> </ul> <note> <p>We strongly recommend using the <code>STANDARD</code> permissions mode to maximize the security of your ledger\
  \ data.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PermissionsMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-update-ledger-permissions-mode-request-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: UpdateLedgerPermissionsModeRequest
---
