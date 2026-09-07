## What

<!-- One or two sentences. The diff already shows the how — say what changed. -->

## Why

<!-- The thing that survives after the diff is forgotten. Link the ADR, ticket, or decision. -->

Closes #

## Verification

<!-- `exit 0` decides — paste the real command and its real output, not "I tested it." -->

```
$
```

- [ ] `pnpm typecheck && pnpm lint && pnpm test` (app) or `supabase db reset && supabase db lint` (backend) — exit 0
- [ ] If this touches a lint rule or RLS policy: I watched it fail on a deliberate violation, then pass once fixed.
- [ ] If this touches a public interface (`data/ports/*`, an exported type, a migration): it's documented; nothing else grew a comment.
