# Content Architecture — Dataset

A synthetic dataset demonstrating how topics can be mapped into a structured SEO content architecture.

## Purpose

The dataset represents a simplified content architecture for a travel website.

It demonstrates relationships between:

- Main topics
- Pillar pages
- Cluster pages
- Supporting pages
- Search intent
- Parent topics
- Internal linking targets

## Dataset Structure

| Field | Description |
|---|---|
| `architecture_id` | Unique architecture record |
| `topic` | Topic represented by the page |
| `page_role` | Pillar, Cluster, or Supporting |
| `parent_topic` | Parent topic |
| `search_intent` | Intended search intent |
| `target_page` | Proposed page |
| `primary_relationship` | Main relationship to another page |
| `internal_link_target` | Suggested related page |
| `status` | Current architecture status |

## Page Roles

### Pillar

Broad topic that acts as the main content hub.

### Cluster

Focused subtopic supporting a pillar.

### Supporting

Narrower topic supporting a cluster or addressing a specific search need.

## Data Principles

The dataset follows these principles:

- Each page has a defined role.
- Each page has a primary topic.
- Parent-child relationships are explicit.
- Search intent is considered when assigning page roles.
- Internal linking targets are contextually related.
- Potential overlap should be reviewed before implementation.

## Limitations

The dataset is synthetic and created for portfolio demonstration purposes.

It does not represent a real website's private content strategy.
