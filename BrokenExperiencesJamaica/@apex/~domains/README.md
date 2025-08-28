# Domain Contexts

Each `~context` represents a bounded context in Domain-Driven Design:

## ~identity.context
Authentication and user identity management
- `.aggregates/` - User, Session, Credential entities
- `.sagas/` - Multi-step authentication flows
- `.projections/` - Read models for auth state
- `.policies/` - Business rules for authentication

## ~reporting.context
Issue reporting and evidence management
- `.aggregates/` - Issue, Evidence, Location entities
- `.workflows/` - Submission and validation pipelines
- `.validators/` - Domain-specific validation rules
- `.events/` - Domain events (IssueCreated, EvidenceAttached)

## ~engagement.context
User engagement and gamification
- `.mechanics/` - Points, badges, leaderboard logic
- `.achievements/` - Achievement definitions and triggers
- `.behaviors/` - User behavior tracking

## ~geospatial.context
Location services and mapping
- `.clustering/` - Map clustering algorithms
- `.heatmaps/` - Issue density visualization
- `.routing/` - Navigation and directions