---
title: "go-graphalgo documentation"
linkTitle: "Home"
type: docs
cascade:
  type: docs
description: "go-graphalgo (planned, wave 3): the graph algorithms gonum lacks, in pure Go (CGO=0): matching, isomorphism, cut extraction, remaining centralities and a MATLAB-style graph facade over gonum/graph, validated against NetworkX."
---

**go-graphalgo is planned, in wave 3.** It holds no library yet: no repository
contains code, and nothing here is released. These pages say what the
organization will cover, which items of the plan it carries, and which
references each package will be validated against.

## Scope

Graph algorithms.

## The plan

In the [go-scikit roadmap](https://github.com/go-scikit/roadmap),
[PLAN.md](https://github.com/go-scikit/roadmap/blob/main/PLAN.md) puts this
organization at item 16 of wave 3 (go-graphalgo: matching, isomorphism, communities, the centralities gonum lacks; gonum/graph already has max flow and betweenness, so they are reused and not rewritten). The plan's rules apply to every item: pure Go (CGO=0) on
every architecture the fleet's CI tests, a bibliography read before any code,
validation against the tools that are the reference in the domain (run as
oracles, never ported when their licence forbids it), unit and regression tests
at 100% coverage, and a performance table against the reference tool.

## Status

[STATUS.md](https://github.com/go-scikit/roadmap/blob/main/STATUS.md) lists
each item of the plan with its repository, pull requests, release and measured
parity. This organization's items are **planned**. The evidence behind the scope
(function inventories, algorithms, reference implementations and licences,
validation oracles) is in the roadmap's
[bibliography](https://github.com/go-scikit/roadmap/blob/main/bib/geometry-pde-graphs.md).

## The planned packages

The package names are working names. None exists as a repository yet.

| Package | Status | What it will provide |
| --- | --- | --- |
| [graph]({{< relref "graph" >}}) | planned (wave 3), no repository yet | Graph algorithms that gonum/graph lacks, behind a MATLAB-style graph and digraph facade. |

## Licences

gonum (BSD-3-Clause) is imported directly and NetworkX (BSD-3-Clause) is the oracle. The igraph C core is GPL-2.0 and is an oracle only; Boost.Graph is BSL-1.0 and permissive.

## Neighbouring organizations

go-graphdrawing (https://github.com/go-graphdrawing) will hold the layouts and depends on this organization. go-sparse supplies sparse matrices for the spectral and Laplacian work.

## What each package's pages hold

| Package | Pages |
| --- | --- |
| graph | [overview]({{< relref "graph" >}}) |
