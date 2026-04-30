# isc-proposal

[![build-status](https://github.com/mufflyt/isoacessr/actions/workflows/publish-proposal.yaml/badge.svg)](https://github.com/mufflyt/isoacessr/actions/workflows/publish-proposal.yaml)

# IsoAccessR

IsoAccessR is a lightweight R package for reproducible geographic
accessibility analysis.

The package focuses on a common workflow: combining travel-time service
areas with population geometries to estimate who can reach a service within a
defined travel time. This workflow is widely used in healthcare, public health,
transportation, and policy, but it is often implemented with custom spatial
code that is hard to reuse or validate.

IsoAccessR provides a small, focused interface for:

- estimating accessibility from service-area polygons
- computing population coverage with area-weighted overlays
- summarizing access across geographies
- producing tidy outputs for downstream analysis

## Proposed R Consortium project

This repository supports the R Consortium ISC proposal:

**IsoAccessR: A Lightweight R Package for Reproducible Accessibility Analysis**

The proposed minimum viable product includes:

- `iso_estimate_access()`
- `iso_summarize_access()`
- one example dataset
- one reproducible vignette
- automated tests and continuous integration

The package is intentionally scoped. It assumes users already have travel-time
polygons. Routing and isochrone generation are out of scope for the first
release.

## Why this matters

Analysts frequently need to estimate population access from service areas, but
they often reimplement area-weighted overlays from scratch. IsoAccessR aims to
reduce that burden by providing a simple, reusable layer above existing R
spatial tools.

## Core dependencies

IsoAccessR is designed to work with:

- `sf`
- `dplyr`
- `testthat`
- `pkgdown`

## Status

Early proposal-stage repository.d under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/RConsortium/isc-
                                                                                                                                                                                                    
                                                                                                                                                                                                    
                                                                                                                                                                                                
                                                                                                                                                                                          proposal" rel="dct:source">https://github.com/RConsortium/isc-proposal</a>.
