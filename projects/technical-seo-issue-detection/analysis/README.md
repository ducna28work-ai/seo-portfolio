# Technical SEO Issue Detection — Analysis

## Analysis Objective

The objective is to demonstrate how technical SEO findings can be organized into issue categories, severity levels, and actionable recommendations.

## Analysis Workflow

**Technical Signal → Issue Detection → Classification → Severity → Recommendation → QA**

## Issue Review

The synthetic dataset includes several technical issue categories:

- HTTP Status
- Indexability
- Canonical
- Redirect
- Metadata
- Internal Linking
- Crawlability

## High-Severity Issues

High-severity examples include:

- 404 responses on important URLs
- 5xx server errors
- Important pages with `noindex`
- Incorrect canonicalization
- Redirect chains affecting important URLs

These issues should generally be reviewed before lower-impact technical improvements.

## Medium-Severity Issues

Examples include:

- Redirect configuration improvements
- Broken internal links
- Missing canonical signals
- Weak internal discoverability

These issues can be addressed according to their affected URL importance and implementation effort.

## Low-Severity Issues

Examples include:

- Missing meta descriptions
- Minor heading structure issues

These improvements can generally be addressed after higher-impact technical problems.

## Detection Principles

A technical SEO finding should be supported by an observable signal.

Examples:

| Finding | Evidence |
|---|---|
| 404 issue | HTTP 404 response |
| 500 issue | HTTP 500 response |
| Noindex issue | `noindex` directive |
| Canonical issue | Canonical target |
| Redirect issue | HTTP 3xx response and destination |
| Broken internal link | Linked URL returns an error |
| Metadata issue | Missing or duplicated element |

## Prioritization

Prioritization should consider:

- SEO impact
- URL importance
- Number of affected URLs
- User impact
- Implementation effort

An issue affecting an important indexable page may receive higher priority than the same technical issue on a low-value URL.

## QA Process

Before closing an issue:

1. Re-check the affected URL.
2. Confirm the technical signal.
3. Confirm the issue classification.
4. Confirm the recommended fix.
5. Verify related URLs where applicable.
6. Re-test after implementation.

## Practical Application

A production workflow could combine:

- Website crawling
- HTTP response analysis
- Robots directive checks
- Canonical extraction
- Redirect analysis
- Internal link validation
- Metadata extraction

The resulting findings can then be filtered and prioritized for implementation.

## Limitations

This analysis uses synthetic technical SEO findings.

It does not represent a live crawl or production website audit.

## Status

The technical SEO issue detection workflow, dataset, and analysis structure are complete.
