---
description: <p>Specifies the type of Amazon Textract features to apply. If you chose <code>TEXTRACT_ANALYZE_DOCUMENT</code> as the read action, you must specify one or both of the following values:</p> <ul> <li> <p> <code>TABLES</code> - Returns additional information about any tables that are detected in the input document. </p> </li> <li> <p> <code>FORMS</code> - Returns additional information about any forms that are detected in the input document. </p> </li> </ul>
layout: schema
name: DocumentReadFeatureTypes
properties_list: []
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-read-feature-types-schema.json
slug: openapi.yml-document-read-feature-types
source_filename: openapi.yml-document-read-feature-types-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-read-feature-types-schema.json\",\n  \"title\": \"DocumentReadFeatureTypes\",\n  \"description\": \"<p>Specifies the type of Amazon Textract features to apply. If you chose <code>TEXTRACT_ANALYZE_DOCUMENT</code> as the read action, you must specify one or both of the following values:</p> <ul> <li> <p> <code>TABLES</code> - Returns additional information about any tables that are detected in the input document. </p> </li> <li> <p> <code>FORMS</code> - Returns additional information about any forms that are detected in the input document. </p> </li> </ul>\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"TABLES\",\n    \"FORMS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-read-feature-types-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentReadFeatureTypes
---
