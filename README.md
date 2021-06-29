# OpenAPI Specifications #

This repository contains [OpenAPI](https://www.openapis.org/) descriptions for [Sitewide's REST API](https://sitewide.dev).

## What is OpenAPI? ##

From the [OpenAPI Specification](https://github.com/OAI/OpenAPI-Specification):

> The OpenAPI Specification (OAS) defines a standard, programming language-agnostic interface description for HTTP APIs, which allows both humans and computers to discover and understand the capabilities of a service without requiring access to source code, additional documentation, or inspection of network traffic. When properly defined via OpenAPI, a consumer can understand and interact with the remote service with a minimal amount of implementation logic. Similar to what interface descriptions have done for lower-level programming, the OpenAPI Specification removes guesswork in calling a service.

## Description Formats ##

Each OpenAPI document SHOULD be available in either **bundled** or **dereferenced** formats.

  - The bundled descriptions are single file artifacts that make usages of OpenAPI **components** for reuse and portability. This SHOULD be the preferred way for 3rd-party developers to interact with Sitewide's OpenAPI description.
  - Certain tools have poor support for references to components within the artifact. Since it is not always possible to switch to tools that fully support referenced components, a fully dereferenced version MAY be provided as well, without any references.

## Vendor Extensions ##

Vendor extensions are used for concepts that are harder to express with OpenAPI components and/or are specific to Sitewide. For more information on the extensions used in these description, please refer to [EXTENSIONS.md](EXTENSIONS.md)

## Limitations ##

  - Not all (optional) HTTP headers are described in the OpenAPI documents, expect those to be added over time.
  - A lot of operations described in these documents are accessible through multiple paths. At a minimum, the most common path is provided to access these operations, but are working on a way to describe alias paths and/or describe all possible paths.

## License ##

sitewide/OAS is licensed under the [Apache License 2.0](LICENSE)
