# Keyword Cannibalization Analysis

A practical project demonstrating how to identify potential keyword cannibalization between website URLs, compare search intent, assess content overlap, and recommend appropriate actions.

## Purpose

Keyword cannibalization can occur when multiple URLs target substantially similar topics or search intent.

This project demonstrates a structured process for determining whether related pages should:

- Remain separate
- Be differentiated
- Be consolidated
- Be redirected
- Be repositioned

The objective is not to eliminate every instance of keyword overlap, but to determine whether multiple URLs serve sufficiently distinct search needs.

## Analysis Workflow

**URL Collection → Topic Mapping → Search Intent Comparison → Content Overlap Review → URL Relationship Analysis → Action Recommendation → QA**

## Analysis Areas

### 1. Topic Similarity

Compare the primary topic targeted by each URL.

Similar topics do not automatically mean that pages are cannibalizing each other.

### 2. Search Intent

Compare whether pages satisfy the same search intent.

Typical intent categories include:

- Informational
- Commercial Investigation
- Transactional
- Navigational

Search intent is a key factor when determining whether similar topics should have separate URLs.

### 3. Content Overlap

Review whether pages provide substantially similar information.

Potential overlap can occur when:

- The same primary topic is covered repeatedly.
- Pages answer substantially the same user question.
- Two pages target the same stage of the user journey.
- One page duplicates another page's primary purpose.

### 4. URL Relationship

Each URL pair can be classified based on their relationship.

| Relationship | Meaning |
|---|---|
| Distinct | Pages have clearly different purposes |
| Related | Pages cover related topics but serve different needs |
| Potential Overlap | Pages may compete for similar search intent |
| Strong Overlap | Pages have substantially similar purpose and content |

## Action Types

### Keep Separate

Use when pages serve clearly different search intents or user needs.

### Differentiate

Use when pages are related but can be given clearer topic or intent boundaries.

### Consolidate

Use when multiple pages provide substantially similar value and a single stronger page would better serve the topic.

### Redirect

Use when one URL should no longer exist as a separate destination and its relevant value can be transferred to another page.

### Reposition

Use when a page can target a different, more specific search intent without requiring consolidation.

## Analysis Record

Each comparison can be documented using:

| Field | Description |
|---|---|
| `analysis_id` | Unique analysis identifier |
| `url_a` | First URL |
| `url_b` | Second URL |
| `topic_a` | Primary topic of URL A |
| `topic_b` | Primary topic of URL B |
| `intent_a` | Search intent of URL A |
| `intent_b` | Search intent of URL B |
| `overlap_level` | Degree of potential overlap |
| `relationship` | Relationship between the URLs |
| `recommended_action` | Proposed action |
| `rationale` | Reason for the recommendation |
| `qa_status` | Review status |

## Decision Framework

A potential cannibalization issue should be evaluated using multiple signals.

```text
Same Topic?
     ↓
Same Search Intent?
     ↓
Significant Content Overlap?
     ↓
Same User Need?
     ↓
Potential Cannibalization
