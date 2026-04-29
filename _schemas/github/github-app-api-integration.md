---
description: GitHub apps are a new way to extend GitHub. They can be installed directly on organizations and user accounts and granted access to specific repositories. They come with granular permissions and built-in webhooks. GitHub apps are first class actors within GitHub.
layout: schema
name: integration
properties_list:
- description: Unique identifier of the GitHub app
  name: id
  type: integer
- description: The slug name of the GitHub app
  name: slug
  type: string
- description: ''
  name: node_id
  type: string
- description: ''
  name: owner
  type: object
- description: The name of the GitHub app
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: external_url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: The set of permissions for the GitHub app
  name: permissions
  type: object
- description: The list of events for the GitHub app
  name: events
  type: array
- description: The number of installations associated with the GitHub app
  name: installations_count
  type: integer
- description: ''
  name: client_id
  type: string
- description: ''
  name: client_secret
  type: string
- description: ''
  name: webhook_secret
  type: string
- description: ''
  name: pem
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-app-api-integration-schema.json
slug: github-app-api-integration
source_filename: github-app-api-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-integration-schema.json\",\n  \"title\": \"integration\",\n  \"description\": \"GitHub apps are a new way to extend GitHub. They can be installed directly on organizations and user accounts and granted access to specific repositories. They come with granular permissions and built-in webhooks. GitHub apps are first class actors within GitHub.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the GitHub app\",\n      \"example\": 37,\n      \"type\": \"integer\"\n    },\n    \"slug\": {\n      \"description\": \"The slug name of the GitHub app\",\n      \"example\": \"probot-owners\",\n      \"type\": \"string\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDExOkludGVncmF0aW9uMQ==\"\n    },\n    \"owner\"\
  : {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"name\": {\n      \"description\": \"The name of the GitHub app\",\n      \"example\": \"Probot Owners\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"The description of the app.\",\n      \"nullable\": true\n    },\n    \"external_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://example.com\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/apps/super-ci\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-07-08T16:18:44-04:00\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-07-08T16:18:44-04:00\"\n    },\n    \"permissions\": {\n      \"description\": \"The set of permissions\
  \ for the GitHub app\",\n      \"type\": \"object\",\n      \"properties\": {\n        \"issues\": {\n          \"type\": \"string\"\n        },\n        \"checks\": {\n          \"type\": \"string\"\n        },\n        \"metadata\": {\n          \"type\": \"string\"\n        },\n        \"contents\": {\n          \"type\": \"string\"\n        },\n        \"deployments\": {\n          \"type\": \"string\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"issues\": \"read\",\n        \"deployments\": \"write\"\n      }\n    },\n    \"events\": {\n      \"description\": \"The list of events for the GitHub app\",\n      \"example\": [\n        \"label\",\n        \"deployment\"\n      ],\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"installations_count\": {\n      \"description\": \"The number of installations associated with the GitHub app\",\n      \"example\"\
  : 5,\n      \"type\": \"integer\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"example\": \"\\\"Iv1.25b5d1e65ffc4022\\\"\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"example\": \"\\\"1d4b2097ac622ba702d19de498f005747a8b21d3\\\"\"\n    },\n    \"webhook_secret\": {\n      \"type\": \"string\",\n      \"example\": \"\\\"6fba8f2fc8a7e8f2cca5577eddd82ca7586b3b6b\\\"\",\n      \"nullable\": true\n    },\n    \"pem\": {\n      \"type\": \"string\",\n      \"example\": \"\\\"--BEGIN RSA PRIVATE KEY--\\\\nMIIEogIBAAKCAQEArYxrNYD/iT5CZVpRJu4rBKmmze3PVmT/gCo2ATUvDvZTPTey\\\\nxcGJ3vvrJXazKk06pN05TN29o98jrYz4cengG3YGsXPNEpKsIrEl8NhbnxapEnM9\\\\nJCMRe0P5JcPsfZlX6hmiT7136GRWiGOUba2X9+HKh8QJVLG5rM007TBER9/z9mWm\\\\nrJuNh+m5l320oBQY/Qq3A7wzdEfZw8qm/mIN0FCeoXH1L6B8xXWaAYBwhTEh6SSn\\\\nZHlO1Xu1JWDmAvBCi0RO5aRSKM8q9QEkvvHP4yweAtK3N8+aAbZ7ovaDhyGz8r6r\\\\nzhU1b8Uo0Z2ysf503WqzQgIajr7Fry7/kUwpgQIDAQABAoIBADwJp80Ko1xHPZDy\\\\nfcCKBDfIuPvkmSW6KumbsLMaQv1aGdHDwwTGv3t0ixSay8CGlxMRtRDyZPib6SvQ\\\
  \\n6OH/lpfpbMdW2ErkksgtoIKBVrDilfrcAvrNZu7NxRNbhCSvN8q0s4ICecjbbVQh\\\\nnueSdlA6vGXbW58BHMq68uRbHkP+k+mM9U0mDJ1HMch67wlg5GbayVRt63H7R2+r\\\\nVxcna7B80J/lCEjIYZznawgiTvp3MSanTglqAYi+m1EcSsP14bJIB9vgaxS79kTu\\\\noiSo93leJbBvuGo8QEiUqTwMw4tDksmkLsoqNKQ1q9P7LZ9DGcujtPy4EZsamSJT\\\\ny8OJt0ECgYEA2lxOxJsQk2kI325JgKFjo92mQeUObIvPfSNWUIZQDTjniOI6Gv63\\\\nGLWVFrZcvQBWjMEQraJA9xjPbblV8PtfO87MiJGLWCHFxmPz2dzoedN+2Coxom8m\\\\nV95CLz8QUShuao6u/RYcvUaZEoYs5bHcTmy5sBK80JyEmafJPtCQVxMCgYEAy3ar\\\\nZr3yv4xRPEPMat4rseswmuMooSaK3SKub19WFI5IAtB/e7qR1Rj9JhOGcZz+OQrl\\\\nT78O2OFYlgOIkJPvRMrPpK5V9lslc7tz1FSh3BZMRGq5jSyD7ETSOQ0c8T2O/s7v\\\\nbeEPbVbDe4mwvM24XByH0GnWveVxaDl51ABD65sCgYB3ZAspUkOA5egVCh8kNpnd\\\\nSd6SnuQBE3ySRlT2WEnCwP9Ph6oPgn+oAfiPX4xbRqkL8q/k0BdHQ4h+zNwhk7+h\\\\nWtPYRAP1Xxnc/F+jGjb+DVaIaKGU18MWPg7f+FI6nampl3Q0KvfxwX0GdNhtio8T\\\\nTj1E+SnFwh56SRQuxSh2gwKBgHKjlIO5NtNSflsUYFM+hyQiPiqnHzddfhSG+/3o\\\\nm5nNaSmczJesUYreH5San7/YEy2UxAugvP7aSY2MxB+iGsiJ9WD2kZzTUlDZJ7RV\\\\nUzWsoqBR+eZfVJ2FUWWvy8TpSG6trh4dFxImNtKejCR1TREpSiTV3Zb1dmahK9GV\\\
  \\nrK9NAoGAbBxRLoC01xfxCTgt5BDiBcFVh4fp5yYKwavJPLzHSpuDOrrI9jDn1oKN\\\\nonq5sDU1i391zfQvdrbX4Ova48BN+B7p63FocP/MK5tyyBoT8zQEk2+vWDOw7H/Z\\\\nu5dTCPxTIsoIwUw1I+7yIxqJzLPFgR2gVBwY1ra/8iAqCj+zeBw=\\\\n--END RSA PRIVATE KEY--\\\\n\\\"\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"owner\",\n    \"name\",\n    \"description\",\n    \"external_url\",\n    \"html_url\",\n    \"created_at\",\n    \"updated_at\",\n    \"permissions\",\n    \"events\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-integration-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: integration
---
