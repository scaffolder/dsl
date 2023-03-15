# Scaffolder DSL

Industry first modeling language based on developer friendly principles. Built by developers for everyone else...

## Definition

Scaffolder DSL or SDSL is a concise, declarative and narrow domain specific modeling language for everything related to software design, architecture, development, support, maintenance... Model once and plan, design, develop, run, operate anything, everywhere!

Supports structural and behavior modelling of any software development phase and methodology.

## Syntax

From the very early releases SDSL is superset of YAML but later will support many other great modeling languages like PlantUML, OCL, DOT, TOML, UML, TextUML, BPML...

## Why YAML?

YAML is very often used for system configuration and it has always been and will continue to be a complete data serialization language that is perfect for modeling structure of data and is ideal for giving meaningful behavior to various system components and interaction.

It's either you love or hate YAML, but there are also people who "love to hate YAML" and we are working really hard to provide tools to transpile to JSON within your code editor of choice very easily.

## Convention over Configuration

SDSL directly implements [Convention over Configuration](https://en.wikipedia.org/wiki/Convention_over_configuration) as a first principle especially with DRY logic.

## Basic building blocks

We call them "scaffolds" and they are minimal YAML files to model everything from Organizations, Divisions, Platforms, Products, Projects, Apps, Services and etc...

### Organizations

```yaml
# organization.yaml
# SDSL v0.1.0
    name: "Scaffolder Ltd."
    brand: "Scaffolder"
    address: "123 Developer's Nest, Planet Earth"
    description: "Developer first application coding and delivery company, shaping the the future of apps development via AI driven coding assistants"
    website: https://scaffolder.dev/about/company
    email: hello@scaffolder.io
```

### Divisions

### Platforms

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
