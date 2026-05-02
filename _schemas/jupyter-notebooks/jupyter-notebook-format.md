---
description: Schema for a Jupyter notebook document (.ipynb) at nbformat major version 4.
layout: schema
name: Jupyter Notebook (nbformat 4)
properties_list:
- description: ''
  name: nbformat
  type: integer
- description: ''
  name: nbformat_minor
  type: integer
- description: ''
  name: metadata
  type: object
- description: ''
  name: cells
  type: array
provider_name: Jupyter Notebooks
provider_slug: jupyter-notebooks
schema_file: json-schema/jupyter-notebook-format-schema.json
slug: jupyter-notebook-format
source_filename: jupyter-notebook-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/main/json-schema/jupyter-notebook-format-schema.json\",\n  \"title\": \"Jupyter Notebook (nbformat 4)\",\n  \"description\": \"Schema for a Jupyter notebook document (.ipynb) at nbformat major version 4.\",\n  \"type\": \"object\",\n  \"required\": [\"nbformat\", \"nbformat_minor\", \"metadata\", \"cells\"],\n  \"properties\": {\n    \"nbformat\": { \"type\": \"integer\", \"const\": 4 },\n    \"nbformat_minor\": { \"type\": \"integer\", \"minimum\": 0 },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"kernelspec\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"display_name\": { \"type\": \"string\" },\n            \"language\": { \"type\": \"string\" }\n          }\n        },\n        \"language_info\": {\n \
  \         \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"version\": { \"type\": \"string\" },\n            \"mimetype\": { \"type\": \"string\" },\n            \"file_extension\": { \"type\": \"string\" }\n          }\n        },\n        \"title\": { \"type\": \"string\" },\n        \"authors\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": { \"name\": { \"type\": \"string\" } }\n          }\n        }\n      }\n    },\n    \"cells\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"oneOf\": [\n          {\n            \"type\": \"object\",\n            \"required\": [\"cell_type\", \"source\"],\n            \"properties\": {\n              \"cell_type\": { \"const\": \"markdown\" },\n              \"metadata\": { \"type\": \"object\" },\n              \"source\": { \"type\": [\"string\", \"array\"] },\n              \"attachments\"\
  : { \"type\": \"object\" }\n            }\n          },\n          {\n            \"type\": \"object\",\n            \"required\": [\"cell_type\", \"source\"],\n            \"properties\": {\n              \"cell_type\": { \"const\": \"raw\" },\n              \"metadata\": { \"type\": \"object\" },\n              \"source\": { \"type\": [\"string\", \"array\"] }\n            }\n          },\n          {\n            \"type\": \"object\",\n            \"required\": [\"cell_type\", \"source\", \"outputs\", \"execution_count\"],\n            \"properties\": {\n              \"cell_type\": { \"const\": \"code\" },\n              \"metadata\": { \"type\": \"object\" },\n              \"source\": { \"type\": [\"string\", \"array\"] },\n              \"execution_count\": { \"type\": [\"integer\", \"null\"] },\n              \"outputs\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"required\": [\"output_type\"\
  ],\n                  \"properties\": {\n                    \"output_type\": {\n                      \"type\": \"string\",\n                      \"enum\": [\"stream\", \"display_data\", \"execute_result\", \"error\"]\n                    }\n                  }\n                }\n              }\n            }\n          }\n        ]\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebooks/refs/heads/main/json-schema/jupyter-notebook-format-schema.json
tags:
- Data Science
- Interactive Computing
- Jupyter
- Notebooks
- Python
title: Jupyter Notebook (nbformat 4)
---
