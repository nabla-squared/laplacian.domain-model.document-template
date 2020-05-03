<!-- @head-content@ -->
# laplacian/domain-model.document-template

This template generates diagrams that represents the structure of schemas
defined by the [Metamodel](https://github.com/nabla-squared/laplacian.model.metamodel).


*Read this in other languages*: [[日本語](README_ja.md)] [[简体中文](README_zh.md)]
<!-- @head-content@ -->

<!-- @toc@ -->
## Table of contents
1. [Usage](#Usage)
1. [Index](#Index)


<!-- @toc@ -->

<!-- @main-content@ -->
## Usage

To apply this Template module, add the following entry to your project definition.
```yaml
project:
  templates:
  - group: laplacian
    name: domain-model.document-template
    version: 1.0.0
```

You can run the following command to see a list of resources affected by the application of this module and their contents.
```console
$ ./script/generate --dry-run

diff --color -r PROJECT_HOME/.NEXT/somewhere/something.md PROJECT_HOME/somewhere/something.md
1,26c1,10
< content: OLD CONTENT
---
> content: NEW CONTENT
```

If there is no problem, execute the following command to reflect the change.
```console
$ ./script/generate --dry-run

```


## Index


### Source code list


- [model/project.yaml](<./model/project.yaml>)
- [src/doc/entities/{each entities.in_namespace as entity}{entity.class_name}.md.hbs](<./src/doc/entities/{each entities.in_namespace as entity}{entity.class_name}.md.hbs>)
- [src/doc/image/model-diagram.puml.hbs](<./src/doc/image/model-diagram.puml.hbs>)
- [src/model/project/document/sections/{if project.domain_model}overview.hbs.yaml](<./src/model/project/document/sections/{if project.domain_model}overview.hbs.yaml>)


<!-- @main-content@ -->