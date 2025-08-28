# Broken Experiences Jamaica - Expert-Level Folder Structure

```
broken-experiences-jamaica/
│
├── .orchestration/                    # Meta-level orchestration & tooling
│   ├── .manifests/                   # K8s-style manifests for local dev
│   ├── .telemetry/                   # OTel configs & custom spans
│   └── .chaos/                       # Chaos engineering scenarios
│
├── @apex/                            # Top-level mobile experiences
│   ├── .native.runtime/              # React Native runtime configs
│   │   ├── .metro.quantum/           # Advanced Metro bundler mods
│   │   └── .hermes.optimized/        # Hermes bytecode caching
│   │
│   ├── ~domains/                     # Domain-driven vertical slices
│   │   ├── ~identity.context/        # Authentication & identity bounded context
│   │   │   ├── .aggregates/          # User, Session, Credential
│   │   │   ├── .sagas/              # Multi-step auth flows
│   │   │   ├── .projections/        # Read models for auth state
│   │   │   └── .policies/           # Auth business rules
│   │   │
│   │   ├── ~reporting.context/       # Issue reporting bounded context
│   │   │   ├── .aggregates/         # Issue, Evidence, Location
│   │   │   ├── .workflows/          # Submission pipelines
│   │   │   ├── .validators/         # Domain validation rules
│   │   │   └── .events/             # Domain events
│   │   │
│   │   ├── ~engagement.context/      # User engagement & gamification
│   │   │   ├── .mechanics/          # Points, badges, leaderboards
│   │   │   ├── .achievements/       # Achievement definitions
│   │   │   └── .behaviors/          # Behavioral tracking
│   │   │
│   │   └── ~geospatial.context/      # Location & mapping
│   │       ├── .clustering/         # Map clustering algorithms
│   │       ├── .heatmaps/          # Issue density visualization
│   │       └── .routing/           # Navigation services
│   │
│   ├── _shells/                      # App shell variations
│   │   ├── _progressive/             # PWA shell
│   │   ├── _native/                 # Pure native shell
│   │   └── _hybrid/                 # WebView hybrid shell
│   │
│   └── §navigation/                  # Navigation orchestration
│       ├── .graphs/                  # Navigation state machines
│       ├── .guards/                  # Route protection
│       └── .transitions/             # Custom animations
│
├── ∞packages/                        # Shared packages (infinity symbol for reusability)
│   ├── @core/                        # Core business logic
│   │   ├── kernel/                   # Domain kernel
│   │   │   ├── .entities/            # Core entities
│   │   │   ├── .valueobjects/       # Immutable value objects
│   │   │   └── .specifications/     # Business rule specs
│   │   │
│   │   ├── contracts/                # Interface definitions
│   │   │   ├── .ports/              # Hexagonal architecture ports
│   │   │   ├── .adapters/           # Implementation adapters
│   │   │   └── .anticorruption/     # ACL patterns
│   │   │
│   │   └── invariants/               # Cross-cutting concerns
│   │       ├── .security/           # Security policies
│   │       ├── .validation/         # Validation rules
│   │       └── .sanitization/       # Input sanitization
│   │
│   ├── @quantum-ui/                  # Advanced UI system
│   │   ├── .atoms/                   # Atomic design atoms
│   │   ├── .molecules/               # Composite components
│   │   ├── .organisms/               # Complex components
│   │   ├── .templates/               # Layout templates
│   │   └── .dimensions/              # Responsive system
│   │
│   ├── @neural-api/                  # Smart API layer
│   │   ├── .graphql.federated/       # GraphQL federation
│   │   ├── .rest.hateoas/           # HATEOAS REST
│   │   ├── .websocket.reactive/     # Reactive streams
│   │   └── .grpc.services/          # gRPC for internal
│   │
│   └── @matrix-state/                # State management matrix
│       ├── .stores/                  # State stores
│       ├── .selectors/              # Memoized selectors
│       ├── .effects/                # Side effect handlers
│       └── .machines/               # XState machines
│
├── ◊supabase/                        # Supabase backend (diamond for data)
│   ├── .genesis/                     # Database initialization
│   │   ├── .schemas/                # Schema definitions
│   │   ├── .seeds/                  # Seed data
│   │   └── .migrations/             # Version migrations
│   │
│   ├── .oracles/                     # Edge Functions (wisdom providers)
│   │   ├── λ.auth-orchestrator/     # Auth flow orchestration
│   │   ├── λ.profile-alchemist/     # Profile transformation
│   │   ├── λ.notification-mesh/     # Notification fanout
│   │   ├── λ.ai-consciousness/      # AI/ML integrations
│   │   ├── λ.media-transcoder/      # Media processing
│   │   └── λ.payment-reconciler/    # Payment processing
│   │
│   ├── .policies/                    # RLS policies
│   │   ├── .row-level/              # Row security
│   │   ├── .column-level/           # Column security
│   │   └── .function-level/         # Function security
│   │
│   ├── .streams/                     # Event streams
│   │   ├── .publishers/             # Event publishers
│   │   ├── .subscribers/            # Event subscribers
│   │   └── .transformers/           # Stream processors
│   │
│   └── .quantum-storage/             # Advanced storage patterns
│       ├── .buckets/                # Storage buckets
│       ├── .cdn-rules/             # CDN configurations
│       └── .transformations/        # Image/video transforms
│
├── ∆infrastructure/                  # Infrastructure as code (delta for change)
│   ├── .terraform-modules/           # IaC modules
│   ├── .pulumi-stacks/              # Alternative IaC
│   ├── .observability/              # Monitoring setup
│   └── .resilience/                 # Fault tolerance
│
├── ¬testing/                         # Testing universes (negation for coverage)
│   ├── .unit-particles/              # Unit tests
│   ├── .integration-waves/          # Integration tests
│   ├── .e2e-journeys/               # End-to-end tests
│   ├── .contract-bonds/             # Contract tests
│   ├── .mutation-evolution/         # Mutation testing
│   ├── .property-generators/        # Property-based tests
│   └── .quantum-scenarios/          # Quantum testing
│
├── ≈analytics/                       # Analytics & insights (approximately)
│   ├── .telemetry-collectors/       # Data collection
│   ├── .event-processors/           # Event processing
│   ├── .ml-pipelines/              # ML pipelines
│   └── .dashboards/                # Visualization
│
├── ⊕devops/                         # DevOps toolchain (addition/composition)
│   ├── .ci-matrices/                # CI/CD pipelines
│   ├── .deployment-strategies/      # Deploy patterns
│   ├── .rollback-procedures/        # Rollback plans
│   └── .sre-playbooks/             # SRE runbooks
│
├── ∂docs/                           # Documentation (partial derivative)
│   ├── .architecture-decisions/     # ADRs
│   ├── .api-specifications/        # OpenAPI/AsyncAPI
│   ├── .user-journeys/             # UX documentation
│   └── .knowledge-graphs/          # Domain knowledge
│
├── ℧experiments/                    # Experimental features (mho/siemens)
│   ├── .feature-flags/             # Feature toggles
│   ├── .a-b-tests/                # A/B testing
│   ├── .canary-releases/          # Canary deployments
│   └── .beta-features/            # Beta programs
│
└── ∇tooling/                       # Developer tooling (nabla operator)
    ├── .code-generators/           # Code generation
    ├── .linters-formatters/        # Code quality
    ├── .git-hooks/                # Git automation
    └── .dev-containers/           # Development environments
```

## Naming Convention Legend

- `@` - Scoped packages/modules
- `~` - Domain contexts (DDD)
- `.` - Hidden/internal directories
- `_` - Shell/wrapper components
- `§` - Cross-cutting concerns
- `λ` - Functions/lambdas
- `∞` - Reusable/infinite use
- `◊` - Data layer (diamond)
- `∆` - Change/infrastructure
- `¬` - Testing (negation/coverage)
- `≈` - Analytics (approximation)
- `⊕` - DevOps (composition)
- `∂` - Documentation (derivative)
- `℧` - Experiments (conductance)
- `∇` - Tools (gradient/nabla)

## Key Architectural Patterns

1. **Hexagonal Architecture** - Ports and adapters in contracts
2. **Domain-Driven Design** - Bounded contexts with aggregates
3. **Event Sourcing Ready** - Event streams and projections
4. **CQRS** - Separate read/write models
5. **Saga Pattern** - Long-running transactions
6. **Micro-frontends** - Domain-based UI slicing
7. **Feature Flags** - Progressive rollouts
8. **Chaos Engineering** - Resilience testing
9. **GitOps Ready** - Declarative infrastructure
10. **Observability First** - Built-in telemetry