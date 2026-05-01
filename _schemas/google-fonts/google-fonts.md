---
description: JSON Schema for the Google Fonts Developer API response objects.
layout: schema
name: Google Fonts Developer API Schema
properties_list: []
provider_name: Google Fonts Developer
provider_slug: google-fonts
schema_file: json-schema/google-fonts.json
slug: google-fonts
source_filename: google-fonts.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-fonts/refs/heads/main/json-schema/google-fonts.json\",\n  \"title\": \"Google Fonts Developer API Schema\",\n  \"description\": \"JSON Schema for the Google Fonts Developer API response objects.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"WebfontList\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"const\": \"webfonts#webfontList\"\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Webfont\"\n          }\n        }\n      }\n    },\n    \"Webfont\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"family\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the font family.\"\n        },\n        \"variants\": {\n          \"type\": \"array\"\
  ,\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Available font variants.\"\n        },\n        \"subsets\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Supported character subsets.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the font family.\"\n        },\n        \"lastModified\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date the font was last modified.\"\n        },\n        \"files\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"description\": \"Map of variant names to font file URLs.\"\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"enum\": [\"serif\",\
  \ \"sans-serif\", \"monospace\", \"display\", \"handwriting\"],\n          \"description\": \"The category of the font.\"\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"const\": \"webfonts#webfont\"\n        },\n        \"axes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Axis\"\n          },\n          \"description\": \"Variable font axes.\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Font tags.\"\n        }\n      }\n    },\n    \"Axis\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tag\": {\n          \"type\": \"string\",\n          \"description\": \"The axis tag (e.g., wght, wdth).\"\n        },\n        \"start\": {\n          \"type\": \"number\",\n          \"description\": \"Minimum value of the axis.\"\n        },\n        \"end\": {\n          \"type\"\
  : \"number\",\n          \"description\": \"Maximum value of the axis.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-fonts/refs/heads/main/json-schema/google-fonts.json
tags:
- CSS
- Design
- Fonts
- Google Fonts
- Typography
- Web Fonts
title: Google Fonts Developer API Schema
---
