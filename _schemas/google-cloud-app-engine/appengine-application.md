---
description: Represents an App Engine application resource, including its configuration, services, and serving status.
layout: schema
name: Google Cloud App Engine Application
properties_list:
- description: Full path to the Application resource in the API.
  name: name
  type: string
- description: Identifier of the Application resource, equivalent to the project ID.
  name: id
  type: string
- description: Google Apps authentication domain that controls which users can access the application.
  name: authDomain
  type: string
- description: Location from which this application runs.
  name: locationId
  type: string
- description: Google Cloud Storage bucket used to store application code.
  name: codeBucket
  type: string
- description: Google Cloud Storage bucket for default storage.
  name: defaultBucket
  type: string
- description: Current serving status of the application.
  name: servingStatus
  type: string
- description: Hostname used to reach this application.
  name: defaultHostname
  type: string
- description: The Google Container Registry domain used for storing managed build docker images.
  name: gcrDomain
  type: string
- description: HTTP path dispatch rules for requests to the application.
  name: dispatchRules
  type: array
provider_name: Google Cloud App Engine
provider_slug: google-cloud-app-engine
schema_file: json-schema/appengine-application.json
slug: appengine-application
source_filename: appengine-application.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/google-cloud-app-engine/refs/heads/main/json-schema/appengine-application.json\",\n  \"title\": \"Google Cloud App Engine Application\",\n  \"description\": \"Represents an App Engine application resource, including its configuration, services, and serving status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full path to the Application resource in the API.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the Application resource, equivalent to the project ID.\"\n    },\n    \"authDomain\": {\n      \"type\": \"string\",\n      \"description\": \"Google Apps authentication domain that controls which users can access the application.\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Location from\
  \ which this application runs.\"\n    },\n    \"codeBucket\": {\n      \"type\": \"string\",\n      \"description\": \"Google Cloud Storage bucket used to store application code.\"\n    },\n    \"defaultBucket\": {\n      \"type\": \"string\",\n      \"description\": \"Google Cloud Storage bucket for default storage.\"\n    },\n    \"servingStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current serving status of the application.\",\n      \"enum\": [\n        \"UNSPECIFIED\",\n        \"SERVING\",\n        \"USER_DISABLED\",\n        \"SYSTEM_DISABLED\"\n      ]\n    },\n    \"defaultHostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname used to reach this application.\"\n    },\n    \"gcrDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The Google Container Registry domain used for storing managed build docker images.\"\n    },\n    \"dispatchRules\": {\n      \"type\": \"array\",\n      \"description\": \"HTTP path dispatch\
  \ rules for requests to the application.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"domain\": {\n            \"type\": \"string\"\n          },\n          \"path\": {\n            \"type\": \"string\"\n          },\n          \"service\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-app-engine/refs/heads/main/json-schema/appengine-application.json
tags:
- App Engine
- Compute
- Google Cloud
- PaaS
- Serverless
- Web Applications
title: Google Cloud App Engine Application
---
