# Technical SEO Issue Detection

A practical project demonstrating a structured workflow for detecting, classifying, prioritizing, and documenting technical SEO issues across website URLs.

## Purpose

Technical SEO issue detection helps identify problems that may affect:

- Crawling
- Indexing
- URL accessibility
- Canonicalization
- Redirect behavior
- Metadata
- Internal linking
- Page status
- Search engine discoverability

The objective is to turn technical findings into clear, actionable recommendations.

## Detection Workflow

**URL Collection → Crawl / Inspection → Issue Detection → Classification → Priority → Recommendation → QA**

## Detection Areas

### 1. Crawlability

Review whether URLs can be accessed and crawled as expected.

Examples:

- 4xx responses
- 5xx responses
- Unexpected redirects
- Redirect chains
- Blocked resources

### 2. Indexability

Review signals that influence whether a page can be indexed.

Examples:

- `noindex`
- Canonical conflicts
- Incorrect canonical URLs
- Indexable pages with unexpected directives

### 3. URL Status

Review HTTP response behavior.

Examples:

- 200 OK
- 3xx redirects
- 4xx errors
- 5xx server errors

### 4. Canonicalization

Review whether canonical signals are consistent with the intended indexable URL.

Potential issues include:

- Missing canonical
- Self-referencing canonical missing
- Canonical pointing to another URL
- Canonical conflicts

### 5. Redirects

Review:

- Redirect destination
- Redirect chains
- Redirect loops
- Unexpected redirect behavior

### 6. On-Page Technical Elements

Review important technical elements such as:

- Title tag
- Meta description
- H1
- Robots directives
- Canonical tag

## Issue Classification

Issues can be classified into:

| Issue Type | Description |
|---|---|
| Crawlability | Problems affecting crawler access |
| Indexability | Problems affecting index eligibility |
| HTTP Status | Unexpected server response |
| Canonical | Incorrect or conflicting canonical signals |
| Redirect | Redirect chain, loop, or incorrect destination |
| Metadata | Missing or problematic technical metadata |
| Internal Linking | Broken or problematic internal links |

## Issue Record

Each finding can be documented using:

| Field | Description |
|---|---|
| `issue_id` | Unique issue identifier |
| `url` | Affected URL |
| `issue_type` | Technical issue category |
| `http_status` | Observed HTTP status |
| `severity` | Issue severity |
| `issue` | Identified problem |
| `evidence` | Observable technical signal |
| `recommendation` | Recommended action |
| `qa_status` | Review status |

## Severity

### High

Issues that may materially affect crawling, indexing, or important URLs.

### Medium

Issues that can negatively affect technical quality or SEO signals but do not necessarily prevent crawling or indexing.

### Low

Minor technical improvements or issues with limited direct SEO impact.

## Detection Principles

Technical findings should be based on observable signals rather than assumptions.

Examples of useful evidence include:

- HTTP response status
- Robots directive
- Canonical target
- Redirect destination
- URL relationship
- Presence or absence of technical elements

## Recommendation Framework

Each issue should answer:

1. What is wrong?
2. What technical signal identifies the issue?
3. Why does the issue matter?
4. What action should be taken?
5. What should be checked after implementation?

## Quality Assurance

Before finalizing an issue:

- Confirm the affected URL.
- Confirm the technical signal.
- Confirm the issue classification.
- Confirm severity.
- Confirm the recommendation addresses the issue.
- Check whether related URLs are affected.
- Verify the issue after implementation.

## Limitations

The dataset used in this project is synthetic and created for portfolio demonstration purposes.

It does not represent private client data, confidential infrastructure information, or production crawl data.

## Status

The technical SEO issue detection framework and synthetic dataset have been established.
