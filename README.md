# OpentelemetryAvalanche

[![CI](https://github.com/HGInsights/opentelemetry_avalanche/actions/workflows/elixir-ci.yml/badge.svg)](https://github.com/HGInsights/opentelemetry_avalanche/actions/workflows/elixir-ci.yml)
[![hex.pm version](https://img.shields.io/hexpm/v/opentelemetry_avalanche.svg)](https://hex.pm/packages/opentelemetry_avalanche)
[![hex.pm license](https://img.shields.io/hexpm/l/opentelemetry_avalanche.svg)](https://github.com/HGInsights/opentelemetry_avalanche/blob/main/LICENSE)
[![Last Updated](https://img.shields.io/github/last-commit/HGInsights/opentelemetry_avalanche.svg)](https://github.com/HGInsights/opentelemetry_avalanche/commits/main)

<!-- MDOC !-->

  `OpentelemetryAvalanche` uses Elixir [telemetry](https://hexdocs.pm/telemetry/) handlers to create [OpenTelemetry](https://opentelemetry.io/) spans from [Avalanche](https://github.com/HGInsights/avalanche)
(Avalanche) query events.

  Currently it supports Avalanche query events: start, stop, exception.

## Usage

Add `:opentelemetry_avalanche` to your dependencies:

```elixir
def deps() do
  [
    {:avalanche, "~> 0.9.1"},
    {:opentelemetry_avalanche, "~> 0.1.0"}
  ]
end
```

Make sure you are using the latest version!

In your application start:

```elixir
def start(_type, _args) do
  OpentelemetryAvalanche.setup()

  # ...
end
```

<!-- MDOC !-->



## Documentation

Documentation is automatically published to
[hexdocs.pm](https://hexdocs.pm/opentelemetry_avalanche) on release. You may build the
documentation locally with

```
MIX_ENV=docs mix docs
```

## Contributing

Issues and PRs are welcome! See our organization [CONTRIBUTING.md](https://github.com/HGInsights/.github/blob/main/CONTRIBUTING.md) for more information about best-practices and passing CI.
