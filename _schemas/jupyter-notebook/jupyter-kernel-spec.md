---
description: Schema for Jupyter kernel specifications (kernelspecs). A kernelspec defines how to launch a specific type of computational kernel, including the command, language, display name, and associated resources.
layout: schema
name: Jupyter Kernel Specification
properties_list:
- description: Unique name of the kernel specification (e.g., 'python3', 'ir', 'julia-1.9').
  name: name
  type: string
- description: The kernel specification details.
  name: spec
  type: object
- description: Resource files associated with the kernel spec, such as logo images.
  name: resources
  type: object
provider_name: Jupyter Notebook
provider_slug: jupyter-notebook
schema_file: json-schema/jupyter-kernel-spec.json
slug: jupyter-kernel-spec
source_filename: jupyter-kernel-spec.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jupyter-kernel-spec.json\",\n  \"title\": \"Jupyter Kernel Specification\",\n  \"description\": \"Schema for Jupyter kernel specifications (kernelspecs). A kernelspec defines how to launch a specific type of computational kernel, including the command, language, display name, and associated resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the kernel specification (e.g., 'python3', 'ir', 'julia-1.9').\"\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"The kernel specification details.\",\n      \"properties\": {\n        \"argv\": {\n          \"type\": \"array\",\n          \"description\": \"Command and arguments to launch the kernel. The special string '{connection_file}' is replaced with the path to the kernel's connection file.\",\n          \"items\": {\n      \
  \      \"type\": \"string\"\n          },\n          \"minItems\": 1\n        },\n        \"display_name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name for the kernel, shown in UIs.\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"The programming language of the kernel (e.g., 'python', 'R', 'julia').\"\n        },\n        \"interrupt_mode\": {\n          \"type\": \"string\",\n          \"description\": \"How the kernel handles interrupts.\",\n          \"enum\": [\"signal\", \"message\"],\n          \"default\": \"signal\"\n        },\n        \"env\": {\n          \"type\": \"object\",\n          \"description\": \"Environment variables to set when launching the kernel.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Additional metadata about the kernel.\"\
  ,\n          \"properties\": {\n            \"debugger\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the kernel supports debugging.\"\n            }\n          },\n          \"additionalProperties\": true\n        }\n      },\n      \"required\": [\"argv\", \"display_name\", \"language\"],\n      \"additionalProperties\": true\n    },\n    \"resources\": {\n      \"type\": \"object\",\n      \"description\": \"Resource files associated with the kernel spec, such as logo images.\",\n      \"properties\": {\n        \"logo-32x32\": {\n          \"type\": \"string\",\n          \"description\": \"Path or URL to the 32x32 pixel kernel logo.\"\n        },\n        \"logo-64x64\": {\n          \"type\": \"string\",\n          \"description\": \"Path or URL to the 64x64 pixel kernel logo.\"\n        },\n        \"logo-svg\": {\n          \"type\": \"string\",\n          \"description\": \"Path or URL to the SVG kernel logo.\"\n        }\n      },\n     \
  \ \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"name\", \"spec\", \"resources\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/json-schema/jupyter-kernel-spec.json
tags:
- Data Science
- Interactive Computing
- Jupyter
- Machine Learning
- Notebooks
- Python
title: Jupyter Kernel Specification
---
