# Absinthe

[GraphQL](https://facebook.github.io/graphql/) implementation for Elixir.

[![Build Status](https://github.com/absinthe-graphql/absinthe/workflows/CI/badge.svg)](https://github.com/absinthe-graphql/absinthe/actions?query=workflow%3ACI)
[![Hex pm](http://img.shields.io/hexpm/v/absinthe.svg)](https://hex.pm/packages/absinthe)
[![Hex Docs](https://img.shields.io/badge/hex-docs-lightgreen.svg)](https://hexdocs.pm/absinthe/)
[![Total Download](https://img.shields.io/hexpm/dt/absinthe.svg)](https://hex.pm/packages/absinthe)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Last Updated](https://img.shields.io/github/last-commit/absinthe-graphql/absinthe.svg)](https://github.com/absinthe-graphql/absinthe/commits/master)

Goals:

- Complete implementation of the [GraphQL Working Draft](https://facebook.github.io/graphql).
- An idiomatic, readable, and comfortable API for Elixir developers
- Extensibility based on small parts that do one thing well.
- Detailed error messages and documentation.
- A focus on robustness and production-level performance.

Please see the website at [http://absinthe-graphql.org](http://absinthe-graphql.org).

## Why Use Absinthe?

Absinthe goes far beyond GraphQL specification basics.

### Easy-to-Read, Fast-to-Run Schemas

Absinthe schemas are defined using easy-to-read macros that build and verify
their structure at compile-time, preventing runtime errors and increasing
performance.

### Pluggability

The entire query processing pipeline is configurable. Add, swap out, or remove
the parser, individual validations, or resolution logic at will, even on a
per-document basis.

### Advanced Resolution

Absinthe includes a number of advanced resolution features, to include:

- Asynchronous field resolution
- Batched field resolution (addressing N+1 query problems)
- A resolution plugin system supporting further extensibility

### Safety

- Complexity analysis and configurable limiting
- Support for precompiled documents/preventing custom documents

### Idiomatic Documents, Idiomatic Code

Write your schemas in idiomatic Elixir `snake_case` notation. Absinthe can
transparently translate to `camelCase` notation for your API clients.

Or, define your own translation schema by writing a simple adapter.

### Frontend Support

We care about support for third-party frameworks, both on the back and
front end.

So far, we include specialized support for Phoenix and Plug on the backend,
and [Relay](https://facebook.github.io/relay/) on the frontend.

Of course we work out of the box with other frontend frameworks and GraphQL
clients, too.

### An Active Community

The project is under constant improvement by a growing list of
contributors, and your feedback is important. Please join us in Slack
(`#absinthe-graphql` under the Elixir Slack account) or the Elixir Forum
(tagged `absinthe`).

Please remember that all interactions in our official spaces follow
our [Code of Conduct](./CODE_OF_CONDUCT.md).

## Installation

Install from [Hex.pm](https://hex.pm/packages/absinthe):

```elixir
def deps do
  [{:absinthe, "~> 1.5.0"}]
end
```

Note: Absinthe requires Elixir 1.4 or higher.

## Upgrading

See [CHANGELOG](./CHANGELOG.md) for upgrade steps between versions.

## Documentation

See [HexDocs](https://hexdocs.pm/absinthe) and <http://absinthe-graphql.org>.

### Mix Tasks

Absinthe includes a number of useful Mix tasks for extracting schema metadata.

Run `mix help` in your project and look for tasks starting with `absinthe`.

### Roadmap

See the [Roadmap project board](https://github.com/absinthe-graphql/absinthe/projects/2) for longer term plans.

## Related Projects

See the [GitHub organization](https://github.com/absinthe-graphql).

## License

See [LICENSE.md](./LICENSE.md).
