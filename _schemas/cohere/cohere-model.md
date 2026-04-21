---
description: Represents a Cohere model with its capabilities, supported endpoints, context length, and configuration details.
layout: schema
name: Cohere Model
properties_list:
- description: The unique name of the model for use in API requests.
  name: name
  type: string
- description: The API endpoints the model is compatible with.
  name: endpoints
  type: array
- description: The maximum number of tokens the model can process in a single request.
  name: context_length
  type: integer
- description: The URL for the model's tokenizer configuration file.
  name: tokenizer_url
  type: string
- description: The API endpoints for which this model is the default selection.
  name: default_endpoints
  type: array
- description: Indicates whether the model is a fine-tuned variant of a base model.
  name: finetuned
  type: boolean
provider_name: cohere
provider_slug: cohere
schema_file: json-schema/cohere-model-schema.json
slug: cohere-model
tags: []
title: Cohere Model
---
