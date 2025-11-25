# Scaffolder DSL

Industry first E2E modeling language based on developer friendly principles. Built by developers for everyone else. A **D**omain **S**pecific **L**anguage for defining entities and processes in the software development domain.

## Definition

Scaffolder DSL or SDSL is a concise, declarative and narrow domain specific modeling language for everything related to software design, architecture, development, support, maintenance... Model once and plan, design, develop, run, operate anything, everywhere!

Supports structural and behavior modelling of any software development phase, process, methodology, tool and more.

## Syntax

From the very early releases SDSL is superset of YAML but later will support many other great modeling languages like PlantUML, OCL, DOT, TOML, UML, TextUML, BPML...

## Why YAML?

YAML is very often used for system configuration and it has always been and will continue to be a complete data serialization language that is perfect for modeling structure of data and is ideal for giving meaningful behavior to various system components and interaction.

It's either you love or hate YAML, but there are also people who "love to hate YAML" and we are working really hard to provide tools to transpile to JSON within your code editor of choice very easily.

## Convention over Configuration

SDSL directly implements [Convention over Configuration](https://en.wikipedia.org/wiki/Convention_over_configuration) as a first principle especially with DRY logic.

## Basic building blocks

We call them "scaffolds" and they are minimal YAML files to model everything from Organizations, Divisions, Platforms, Products, Projects, Apps, Services and etc...
It doesn't matter if project is small or big, whether is greenfield or brownfield, SDSL allows Developers, Architects, Engineers, SRE, DevOps, Platform Engineers and AI Assistants all communicate on a common high level language.

Here are few examples to demonstrate the possibilities:

### Organizations

```yaml
# organization.yaml
# SDSL v0.1.0

name: "Scaffolder Ltd."
brand: "Scaffolder"
address: "123 Developer's Nest, Planet Earth"
description: "Developer first application coding and delivery company, shaping the the future of apps development via AI driven coding assistants"
website: https://scaffolder.io/ # https://scaffolder.dev/about/company
email: hello@scaffolder.io
github: https://github.com/scaffolder
```

### Divisions

```yaml
# division.yaml
# SDSL v0.1.0

name: "Platform Engineering Division"
brand: "Scaffolder Platform"
description: >-
  Focuses on building and maintaining the core platform services,
  CI/CD pipelines, and developer tooling across the global organization.
website: "https://divisions.scaffolder.io/platform"
email: "platform@scaffolder.io"
github: "https://github.com/scaffolder/platform"
head:
  name: "Din Djarin"
  slack: "@din.djarin"
  twitter: "@mandalorian"
  linkedin: "https://linkedin.com/in/din.djarin"
  phone: "+49-30-12345678"
  location: "Mandalore, Outer Rim"
```

### Platforms

```yaml
name: "Application Platform as a Service"
brand: "Scaffolder aPaaS"
description: >-
  Provides a fully managed environment for developers to build,
  deploy, and scale applications with minimal operational overhead.
website: "https://platform.scaffolder.io"
email: "platform@scaffolder.io"
github: "https://github.com/scaffolder/apaaS"
head:
  name: "Ahsoka Tano"
  slack: "@ahsoka.tano"
  twitter: "@ahsoka_tano"
  linkedin: "https://linkedin.com/in/ahsoka.tano"
  phone: "+49-30-98765432"
  location: "Coruscant, Galactic Republic"

services:
  compute:
    type: "Kubernetes"
    version: "1.27"
  storage:
    type: "Object"
    provider: "S3‑compatible"
  database:
    type: "PostgreSQL"
    version: "15"
  messaging:
    type: "Kafka"
    version: "3.5"

pricing:
  tiers:
    free:
      description: "Limited resources for evaluation"
      limits:
        cpu: "1 vCPU"
        memory: "2 GB"
        storage: "5 GB"
    enterprise:
      price_per_hour: 0.12
      currency: "EUR"

regions:
  available: ["eu-central-1", "us-east-1", "ap-southeast-2"]
  default: "eu-central-1"

sla:
  uptime: "99.95%"
  response_time: "≤ 150 ms"
  support_hours: "24/7"

apis:
  rest:
    base_url: "https://api.platform.scaffolder.io"
    version: "v2"
  graphql:
    endpoint: "https://graphql.platform.scaffolder.io"

integrations:
  ci_cd: ["GitHub Actions", "GitLab CI"]
  monitoring: ["Prometheus", "Datadog"]

security:
  compliance: ["ISO‑27001", "SOC‑2"]
  encryption_at_rest: true
  encryption_in_transit: true
  identity_provider: "OIDC"

features:
  auto_scaling: true
  blue_green_deployments: true
  canary_releases: true
  service_mesh: "Istio"
```

### Products

### Projects

### Apps

### Services

### SDLCs

### Workflows

### Steps

### Frameworks

### Processes

### Microservices

### Environments

### Generators

### Templates

...
