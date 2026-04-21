---
description: LanguageDetectionResult schema from Apache OpenNLP
layout: schema
name: LanguageDetectionResult
properties_list:
- description: ISO-639-3 code of most likely language
  name: bestLanguage
  type: string
- description: Confidence score 0-1
  name: confidence
  type: number
- description: All detected languages with probabilities
  name: languages
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-language-detection-result-schema.json
slug: apache-opennlp-language-detection-result
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: LanguageDetectionResult
---
