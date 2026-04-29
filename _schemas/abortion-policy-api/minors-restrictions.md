---
description: Abortion restrictions that specifically target minors in a US state.
layout: schema
name: MinorsRestrictions
properties_list:
- description: Age below which restrictions apply. Null means no restrictions currently enforced.
  name: below_age
  type: integer
- description: Number of parents required to be notified. 1=one parent, 2=both parents, null=no restrictions.
  name: parents_required
  type: integer
- description: If true, parent(s) must give permission for the minor to have an abortion.
  name: parental_consent_required
  type: boolean
- description: If true, parent(s) must be told beforehand of the minor's decision.
  name: parental_notification_required
  type: boolean
- description: If true, a judge can excuse a minor from parental consent/notification requirements.
  name: judicial_bypass_available
  type: boolean
- description: If true, state explicitly or implicitly allows a minor to consent to abortion.
  name: allows_minor_to_consent
  type: boolean
- description: Date this policy record was last updated.
  name: Last Updated
  type: string
provider_name: Abortion Policy API
provider_slug: abortion-policy-api
schema_file: json-schema/minors-restrictions-schema.json
slug: minors-restrictions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/minors-restrictions-schema.json\",\n  \"title\": \"MinorsRestrictions\",\n  \"description\": \"Abortion restrictions that specifically target minors in a US state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"below_age\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Age below which restrictions apply. Null means no restrictions currently enforced.\",\n      \"example\": 18\n    },\n    \"parents_required\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Number of parents required to be notified. 1=one parent, 2=both parents, null=no restrictions.\",\n      \"example\": 1\n    },\n    \"parental_consent_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, parent(s) must give permission\
  \ for the minor to have an abortion.\",\n      \"example\": false\n    },\n    \"parental_notification_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, parent(s) must be told beforehand of the minor's decision.\",\n      \"example\": false\n    },\n    \"judicial_bypass_available\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, a judge can excuse a minor from parental consent/notification requirements.\",\n      \"example\": false\n    },\n    \"allows_minor_to_consent\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, state explicitly or implicitly allows a minor to consent to abortion.\",\n      \"example\": true\n    },\n    \"Last Updated\": {\n      \"type\": \"string\",\n      \"description\": \"Date this policy record was last updated.\",\n      \"example\": \"2025-01-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/minors-restrictions-schema.json
tags:
- Abortion
- Policies
- Healthcare
- Government
title: MinorsRestrictions
---
