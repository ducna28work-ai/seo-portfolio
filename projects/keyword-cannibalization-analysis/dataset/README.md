# Keyword Cannibalization Analysis — Dataset

Synthetic dataset demonstrating how pairs of URLs can be compared for potential keyword cannibalization.

## Dataset Schema

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

## Overlap Levels

- Distinct
- Related
- Potential Overlap
- Strong Overlap

## Recommended Actions

- Keep Separate
- Differentiate
- Consolidate
- Redirect
- Reposition

## Data Principles

Each comparison should consider:

- Topic similarity
- Search intent
- Content purpose
- User need
- URL relationship

Keyword similarity alone should not determine the final recommendation.

## Limitations

All records are synthetic and intended only to demonstrate keyword cannibalization analysis methodology.
