---
description: Core metadata for a Python package hosted on PyPI, as returned by the JSON API. This schema captures the info object that describes authorship, licensing, dependencies, and classification of a project.
layout: schema
name: PyPI Project Metadata
properties_list:
- description: The name of the Python package.
  name: name
  type: string
- description: The version string of the release, following PEP 440.
  name: version
  type: string
- description: A one-line summary of what the package does.
  name: summary
  type:
  - string
  - 'null'
- description: The full description of the package, which may be in reStructuredText, Markdown, or plain text.
  name: description
  type:
  - string
  - 'null'
- description: The content type of the description field.
  name: description_content_type
  type:
  - string
  - 'null'
- description: The name of the package author.
  name: author
  type:
  - string
  - 'null'
- description: The email address of the package author.
  name: author_email
  type:
  - string
  - 'null'
- description: The name of the package maintainer.
  name: maintainer
  type:
  - string
  - 'null'
- description: The email address of the package maintainer.
  name: maintainer_email
  type:
  - string
  - 'null'
- description: The license text or identifier for the package.
  name: license
  type:
  - string
  - 'null'
- description: A SPDX license expression for the package.
  name: license_expression
  type:
  - string
  - 'null'
- description: A list of license file paths included in the distribution.
  name: license_files
  type:
  - array
  - 'null'
- description: Comma-separated keywords describing the package.
  name: keywords
  type:
  - string
  - 'null'
- description: Trove classifiers indicating the package maturity, audience, license, and supported environments.
  name: classifiers
  type: array
- description: The platform the package targets.
  name: platform
  type:
  - string
  - 'null'
- description: The URL of the project home page.
  name: home_page
  type:
  - string
  - 'null'
- description: The canonical URL of the project on PyPI.
  name: project_url
  type: string
- description: A mapping of label strings to URL strings for project-related links.
  name: project_urls
  type:
  - object
  - 'null'
- description: The Python version requirement specifier, following PEP 440.
  name: requires_python
  type:
  - string
  - 'null'
- description: A list of PEP 508 dependency specifiers required by the package.
  name: requires_dist
  type:
  - array
  - 'null'
- description: A list of optional extra dependency groups provided by the package.
  name: provides_extra
  type:
  - array
  - 'null'
- description: Metadata fields that are dynamically specified at build time.
  name: dynamic
  type:
  - array
  - 'null'
- description: Whether this release has been yanked from the index.
  name: yanked
  type: boolean
- description: The reason the release was yanked, if applicable.
  name: yanked_reason
  type:
  - string
  - 'null'
provider_name: PyPI
provider_slug: pypi
schema_file: json-schema/pypi-project-metadata-schema.json
slug: pypi-project-metadata
source_filename: pypi-project-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://pypi.org/schemas/pypi/project-metadata.json\",\n  \"title\": \"PyPI Project Metadata\",\n  \"description\": \"Core metadata for a Python package hosted on PyPI, as returned by the JSON API. This schema captures the info object that describes authorship, licensing, dependencies, and classification of a project.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"version\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Python package.\",\n      \"minLength\": 1,\n      \"pattern\": \"^[a-zA-Z0-9]([a-zA-Z0-9._-]*[a-zA-Z0-9])?$\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version string of the release, following PEP 440.\",\n      \"minLength\": 1\n    },\n    \"summary\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A one-line summary of what the package\
  \ does.\",\n      \"maxLength\": 512\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The full description of the package, which may be in reStructuredText, Markdown, or plain text.\"\n    },\n    \"description_content_type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The content type of the description field.\",\n      \"enum\": [null, \"text/plain\", \"text/x-rst\", \"text/markdown\"]\n    },\n    \"author\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the package author.\"\n    },\n    \"author_email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The email address of the package author.\",\n      \"format\": \"email\"\n    },\n    \"maintainer\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the package maintainer.\"\n    },\n    \"maintainer_email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"The email address of the package maintainer.\",\n      \"format\": \"email\"\n    },\n    \"license\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The license text or identifier for the package.\"\n    },\n    \"license_expression\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A SPDX license expression for the package.\"\n    },\n    \"license_files\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A list of license file paths included in the distribution.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"keywords\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Comma-separated keywords describing the package.\"\n    },\n    \"classifiers\": {\n      \"type\": \"array\",\n      \"description\": \"Trove classifiers indicating the package maturity, audience, license, and supported environments.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\"\
  : \"^[A-Za-z]\"\n      }\n    },\n    \"platform\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The platform the package targets.\"\n    },\n    \"home_page\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The URL of the project home page.\",\n      \"format\": \"uri\"\n    },\n    \"project_url\": {\n      \"type\": \"string\",\n      \"description\": \"The canonical URL of the project on PyPI.\",\n      \"format\": \"uri\"\n    },\n    \"project_urls\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"A mapping of label strings to URL strings for project-related links.\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"requires_python\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Python version requirement specifier, following PEP 440.\"\n    },\n    \"requires_dist\": {\n      \"type\": [\"array\", \"null\"],\n     \
  \ \"description\": \"A list of PEP 508 dependency specifiers required by the package.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"provides_extra\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A list of optional extra dependency groups provided by the package.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"dynamic\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"Metadata fields that are dynamically specified at build time.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"yanked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this release has been yanked from the index.\"\n    },\n    \"yanked_reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The reason the release was yanked, if applicable.\"\n    }\n  },\n  \"$defs\": {\n    \"ReleaseFile\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata\
  \ about a single distribution file within a release.\",\n      \"required\": [\"filename\", \"url\"],\n      \"properties\": {\n        \"filename\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the distribution file.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"The download URL for the distribution file.\",\n          \"format\": \"uri\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n          \"description\": \"The size of the file in bytes.\",\n          \"minimum\": 0\n        },\n        \"packagetype\": {\n          \"type\": \"string\",\n          \"description\": \"The type of distribution.\",\n          \"enum\": [\"sdist\", \"bdist_wheel\", \"bdist_egg\", \"bdist_wininst\", \"bdist_rpm\"]\n        },\n        \"python_version\": {\n          \"type\": \"string\",\n          \"description\": \"The Python version this distribution targets.\"\n        },\n        \"requires_python\"\
  : {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The Python version requirement for this file.\"\n        },\n        \"upload_time_iso_8601\": {\n          \"type\": \"string\",\n          \"description\": \"The ISO 8601 timestamp when the file was uploaded.\",\n          \"format\": \"date-time\"\n        },\n        \"digests\": {\n          \"$ref\": \"#/$defs/Digests\"\n        },\n        \"yanked\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this file has been yanked.\"\n        },\n        \"yanked_reason\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The reason the file was yanked.\"\n        }\n      }\n    },\n    \"Digests\": {\n      \"type\": \"object\",\n      \"description\": \"Cryptographic hash digests for a distribution file.\",\n      \"properties\": {\n        \"md5\": {\n          \"type\": \"string\",\n          \"description\": \"MD5 hash digest of the file.\",\n      \
  \    \"pattern\": \"^[a-f0-9]{32}$\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 hash digest of the file.\",\n          \"pattern\": \"^[a-f0-9]{64}$\"\n        },\n        \"blake2b_256\": {\n          \"type\": \"string\",\n          \"description\": \"BLAKE2b-256 hash digest of the file.\",\n          \"pattern\": \"^[a-f0-9]{64}$\"\n        }\n      }\n    },\n    \"Vulnerability\": {\n      \"type\": \"object\",\n      \"description\": \"A known security vulnerability affecting the project.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the vulnerability, such as a CVE or PYSEC ID.\"\n        },\n        \"aliases\": {\n          \"type\": \"array\",\n          \"description\": \"Alternative identifiers for this vulnerability.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n \
  \       },\n        \"summary\": {\n          \"type\": \"string\",\n          \"description\": \"A brief summary of the vulnerability.\"\n        },\n        \"details\": {\n          \"type\": \"string\",\n          \"description\": \"A detailed description of the vulnerability.\"\n        },\n        \"fixed_in\": {\n          \"type\": \"array\",\n          \"description\": \"Version strings in which the vulnerability was fixed.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"A URL with more information about the vulnerability.\",\n          \"format\": \"uri\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/json-schema/pypi-project-metadata-schema.json
tags:
- Developer Tools
- Open Source
- Package Management
- Packages
- Python
title: PyPI Project Metadata
---
