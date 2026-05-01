---
description: <p>Information about each word or line of text in the input document.</p> <p>For additional information, see <a href="https://docs.aws.amazon.com/textract/latest/dg/API_Block.html">Block</a> in the Amazon Textract API reference.</p>
layout: schema
name: Block
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: BlockType
  type: object
- description: ''
  name: Text
  type: object
- description: ''
  name: Page
  type: object
- description: ''
  name: Geometry
  type: object
- description: ''
  name: Relationships
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-block-schema.json
slug: openapi.yml-block
source_filename: openapi.yml-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-block-schema.json\",\n  \"title\": \"Block\",\n  \"description\": \"<p>Information about each word or line of text in the input document.</p> <p>For additional information, see <a href=\\\"https://docs.aws.amazon.com/textract/latest/dg/API_Block.html\\\">Block</a> in the Amazon Textract API reference.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique identifier for the block.\"\n        }\n      ]\n    },\n    \"BlockType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockType\"\n        },\n        {\n          \"description\": \"<p>The block represents a line of text or one word of text.</p> <ul>\
  \ <li> <p>WORD - A word that's detected on a document page. A word is one or more ISO basic Latin script characters that aren't separated by spaces.</p> </li> <li> <p>LINE - A string of tab-delimited, contiguous words that are detected on a document page</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The word or line of text extracted from the block.\"\n        }\n      ]\n    },\n    \"Page\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Page number where the block appears.\"\n        }\n      ]\n    },\n    \"Geometry\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Geometry\"\n        },\n        {\n          \"description\": \"Co-ordinates of the rectangle or polygon that contains the text.\"\n        }\n  \
  \    ]\n    },\n    \"Relationships\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfRelationships\"\n        },\n        {\n          \"description\": \"A list of child blocks of the current block. For example, a LINE object has child blocks for each WORD block that's part of the line of text. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-block-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: Block
---
