---
description: A Firestore document resource representing a single entity stored in a Firestore collection.
layout: schema
name: Google Cloud Firestore Document
properties_list:
- description: The resource name of the document in the format projects/{project}/databases/{database}/documents/{collection}/{documentId}.
  name: name
  type: string
- description: The document's fields as a map of field names to values.
  name: fields
  type: object
- description: The time at which the document was created.
  name: createTime
  type: string
- description: The time at which the document was last changed.
  name: updateTime
  type: string
provider_name: Google Cloud Firestore
provider_slug: google-cloud-firestore
schema_file: json-schema/document-schema.json
slug: document
source_filename: document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-firestore/refs/heads/main/json-schema/document-schema.json\",\n  \"title\": \"Google Cloud Firestore Document\",\n  \"description\": \"A Firestore document resource representing a single entity stored in a Firestore collection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the document in the format projects/{project}/databases/{database}/documents/{collection}/{documentId}.\",\n      \"pattern\": \"^projects/[^/]+/databases/[^/]+/documents/.+$\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"The document's fields as a map of field names to values.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Value\"\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"The time at which the document was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which the document was last changed.\"\n    }\n  },\n  \"$defs\": {\n    \"Value\": {\n      \"type\": \"object\",\n      \"description\": \"A Firestore value that represents a typed field value.\",\n      \"properties\": {\n        \"nullValue\": {\n          \"type\": \"string\",\n          \"const\": \"NULL_VALUE\",\n          \"description\": \"A null value.\"\n        },\n        \"booleanValue\": {\n          \"type\": \"boolean\",\n          \"description\": \"A boolean value.\"\n        },\n        \"integerValue\": {\n          \"type\": \"string\",\n          \"description\": \"An integer value (as a string for 64-bit precision).\"\n        },\n        \"doubleValue\": {\n          \"type\": \"number\",\n          \"description\": \"A double value.\"\n      \
  \  },\n        \"timestampValue\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"A timestamp value.\"\n        },\n        \"stringValue\": {\n          \"type\": \"string\",\n          \"description\": \"A string value.\"\n        },\n        \"bytesValue\": {\n          \"type\": \"string\",\n          \"contentEncoding\": \"base64\",\n          \"description\": \"A bytes value (base64-encoded).\"\n        },\n        \"referenceValue\": {\n          \"type\": \"string\",\n          \"description\": \"A reference to a document.\"\n        },\n        \"geoPointValue\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"latitude\": {\n              \"type\": \"number\",\n              \"minimum\": -90,\n              \"maximum\": 90\n            },\n            \"longitude\": {\n              \"type\": \"number\",\n              \"minimum\": -180,\n              \"maximum\": 180\n            }\n     \
  \     },\n          \"description\": \"A geo point value.\"\n        },\n        \"arrayValue\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"values\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/Value\"\n              }\n            }\n          },\n          \"description\": \"An array value.\"\n        },\n        \"mapValue\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"fields\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/Value\"\n              }\n            }\n          },\n          \"description\": \"A map value.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-firestore/refs/heads/main/json-schema/document-schema.json
tags:
- Database
- Documents
- Google Cloud
- NoSQL
- Real-Time
title: Google Cloud Firestore Document
---
