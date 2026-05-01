---
description: A volume resource from the Google Books API representing a book or publication.
layout: schema
name: Google Books Volume
properties_list:
- description: ''
  name: kind
  type: string
- description: Unique identifier for the volume.
  name: id
  type: string
- description: ''
  name: etag
  type: string
- description: ''
  name: selfLink
  type: string
- description: General volume information.
  name: volumeInfo
  type: object
- description: ''
  name: saleInfo
  type: object
- description: ''
  name: accessInfo
  type: object
provider_name: Google Books
provider_slug: google-books
schema_file: json-schema/books.json
slug: books
source_filename: books.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-books/refs/heads/main/json-schema/books.json\",\n  \"title\": \"Google Books Volume\",\n  \"description\": \"A volume resource from the Google Books API representing a book or publication.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"books#volume\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the volume.\"\n    },\n    \"etag\": {\n      \"type\": \"string\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"volumeInfo\": {\n      \"type\": \"object\",\n      \"description\": \"General volume information.\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Volume title.\"\n        },\n        \"subtitle\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Volume subtitle.\"\n        },\n        \"authors\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"The names of the authors.\"\n        },\n        \"publisher\": {\n          \"type\": \"string\",\n          \"description\": \"Publisher of this volume.\"\n        },\n        \"publishedDate\": {\n          \"type\": \"string\",\n          \"description\": \"Date of publication.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A synopsis of the volume.\"\n        },\n        \"industryIdentifiers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"ISBN_10\", \"ISBN_13\", \"ISSN\", \"OTHER\"]\n              },\n              \"identifier\"\
  : {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"pageCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of pages.\"\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"A list of subject categories.\"\n        },\n        \"averageRating\": {\n          \"type\": \"number\",\n          \"description\": \"The mean review rating.\"\n        },\n        \"ratingsCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of review ratings.\"\n        },\n        \"imageLinks\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"smallThumbnail\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"thumbnail\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n         \
  \   }\n          }\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"Best language for this volume based on content.\"\n        }\n      },\n      \"required\": [\"title\"]\n    },\n    \"saleInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"country\": { \"type\": \"string\" },\n        \"saleability\": {\n          \"type\": \"string\",\n          \"enum\": [\"FOR_SALE\", \"FREE\", \"NOT_FOR_SALE\", \"FOR_PREORDER\"]\n        },\n        \"isEbook\": { \"type\": \"boolean\" },\n        \"listPrice\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"amount\": { \"type\": \"number\" },\n            \"currencyCode\": { \"type\": \"string\" }\n          }\n        }\n      }\n    },\n    \"accessInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"viewability\": {\n          \"type\": \"string\",\n          \"enum\": [\"PARTIAL\", \"ALL_PAGES\", \"NO_PAGES\", \"UNKNOWN\"\
  ]\n        },\n        \"embeddable\": { \"type\": \"boolean\" },\n        \"publicDomain\": { \"type\": \"boolean\" }\n      }\n    }\n  },\n  \"required\": [\"kind\", \"id\", \"volumeInfo\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-books/refs/heads/main/json-schema/books.json
tags:
- Books
- eBooks
- Google
- Library
- Publishing
- Reading
- Search
title: Google Books Volume
---
