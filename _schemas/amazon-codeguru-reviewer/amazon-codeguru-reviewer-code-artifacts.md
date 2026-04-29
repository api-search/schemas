---
description: <p>Code artifacts are source code artifacts and build artifacts used in a repository analysis or a pull request review.</p> <ul> <li> <p>Source code artifacts are source code files in a Git repository that are compressed into a .zip file.</p> </li> <li> <p>Build artifacts are .jar or .class files that are compressed in a .zip file.</p> </li> </ul>
layout: schema
name: CodeArtifacts
properties_list:
- description: ''
  name: SourceCodeArtifactsObjectKey
  type: object
- description: ''
  name: BuildArtifactsObjectKey
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-code-artifacts-schema.json
slug: amazon-codeguru-reviewer-code-artifacts
source_filename: amazon-codeguru-reviewer-code-artifacts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-artifacts-schema.json\",\n  \"title\": \"CodeArtifacts\",\n  \"description\": \"<p>Code artifacts are source code artifacts and build artifacts used in a repository analysis or a pull request review.</p> <ul> <li> <p>Source code artifacts are source code files in a Git repository that are compressed into a .zip file.</p> </li> <li> <p>Build artifacts are .jar or .class files that are compressed in a .zip file.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceCodeArtifactsObjectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceCodeArtifactsObjectKey\"\n        },\n        {\n          \"description\": \"The S3 object key for a source code .zip file. This is required for all code reviews.\"\n     \
  \   }\n      ]\n    },\n    \"BuildArtifactsObjectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildArtifactsObjectKey\"\n        },\n        {\n          \"description\": \"The S3 object key for a build artifacts .zip file that contains .jar or .class files. This is required for a code review with security analysis. For more information, see <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-ug/working-with-cicd.html\\\">Create code reviews with GitHub Actions</a> in the <i>Amazon CodeGuru Reviewer User Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SourceCodeArtifactsObjectKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-artifacts-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: CodeArtifacts
---
