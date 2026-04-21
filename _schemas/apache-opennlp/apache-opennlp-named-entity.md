---
description: NamedEntity schema from Apache OpenNLP
layout: schema
name: NamedEntity
properties_list:
- description: Entity text
  name: text
  type: string
- description: Entity type
  name: type
  type: string
- description: Start token index
  name: start
  type: integer
- description: End token index (exclusive)
  name: end
  type: integer
- description: Confidence score
  name: probability
  type: number
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-named-entity-schema.json
slug: apache-opennlp-named-entity
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: NamedEntity
---
