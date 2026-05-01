---
description: Schema for a Google Colab notebook file in Jupyter notebook format (.ipynb), containing code cells, text cells, metadata, and execution outputs.
layout: schema
name: Google Colab Notebook
properties_list:
- description: Notebook format major version
  name: nbformat
  type: integer
- description: Notebook format minor version
  name: nbformat_minor
  type: integer
- description: ''
  name: metadata
  type: object
- description: The cells in the notebook
  name: cells
  type: array
provider_name: Google Colab
provider_slug: google-colab
schema_file: json-schema/google-colab-notebook-schema.json
slug: google-colab-notebook
source_filename: google-colab-notebook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://colab.research.google.com/schemas/notebook.json\",\n  \"title\": \"Google Colab Notebook\",\n  \"description\": \"Schema for a Google Colab notebook file in Jupyter notebook format (.ipynb), containing code cells, text cells, metadata, and execution outputs.\",\n  \"type\": \"object\",\n  \"required\": [\"nbformat\", \"nbformat_minor\", \"metadata\", \"cells\"],\n  \"properties\": {\n    \"nbformat\": {\n      \"type\": \"integer\",\n      \"description\": \"Notebook format major version\",\n      \"const\": 4\n    },\n    \"nbformat_minor\": {\n      \"type\": \"integer\",\n      \"description\": \"Notebook format minor version\",\n      \"minimum\": 0\n    },\n    \"metadata\": {\n      \"$ref\": \"#/$defs/NotebookMetadata\"\n    },\n    \"cells\": {\n      \"type\": \"array\",\n      \"description\": \"The cells in the notebook\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Cell\"\
  \n      }\n    }\n  },\n  \"$defs\": {\n    \"NotebookMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Notebook-level metadata including Colab-specific settings\",\n      \"properties\": {\n        \"colab\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The notebook name displayed in Colab\"\n            },\n            \"provenance\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\"\n              }\n            },\n            \"collapsed_sections\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"toc_visible\": {\n              \"type\": \"boolean\"\n            }\n          }\n        },\n        \"kernelspec\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\"\
  : {\n              \"type\": \"string\",\n              \"default\": \"python3\"\n            },\n            \"display_name\": {\n              \"type\": \"string\",\n              \"default\": \"Python 3\"\n            }\n          }\n        },\n        \"language_info\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"default\": \"python\"\n            }\n          }\n        },\n        \"accelerator\": {\n          \"type\": \"string\",\n          \"description\": \"Hardware accelerator type\",\n          \"enum\": [\"GPU\", \"TPU\", \"NONE\"]\n        }\n      }\n    },\n    \"Cell\": {\n      \"type\": \"object\",\n      \"required\": [\"cell_type\", \"source\", \"metadata\"],\n      \"properties\": {\n        \"cell_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"code\", \"markdown\", \"raw\"],\n          \"description\": \"The type of cell\"\n        },\n        \"\
  source\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The source content of the cell as an array of lines\"\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\"\n            },\n            \"colab_type\": {\n              \"type\": \"string\"\n            }\n          },\n          \"additionalProperties\": true\n        },\n        \"execution_count\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Execution count for code cells\"\n        },\n        \"outputs\": {\n          \"type\": \"array\",\n          \"description\": \"Outputs from code cell execution\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Output\"\n          }\n        }\n      }\n    },\n    \"Output\": {\n      \"type\": \"object\",\n      \"description\": \"An output from a code\
  \ cell execution\",\n      \"properties\": {\n        \"output_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"stream\", \"display_data\", \"execute_result\", \"error\"]\n        },\n        \"text\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"enum\": [\"stdout\", \"stderr\"]\n        },\n        \"ename\": {\n          \"type\": \"string\"\n        },\n        \"evalue\": {\n          \"type\": \"string\"\n        },\n        \"traceback\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-colab/refs/heads/main/json-schema/google-colab-notebook-schema.json
tags:
- Collaboration
- Data Science
- Google Cloud
- Jupyter
- Machine Learning
- Notebooks
- Python
title: Google Colab Notebook
---
