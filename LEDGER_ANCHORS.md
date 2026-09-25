# Ledger anchors

External witness for the **artinscience ledger**, the private system of record
behind the work: research rights, plot telemetry, plates and sales. Each entry
below is a reproducible sha256 over the ledger's append-only audit tables at a
point in time.

Committing the digest here, in a public repository whose history is
human-reviewed and human-merged, anchors the private ledger to a timeline it
cannot rewrite: any later tampering with the audit tables would break the
digest chain against these commits.

**The habit:** after meaningful ledger activity (a plot session, a sale, a
rights backfill), compute a new digest anchored to the merge commit of the
*previous* entry here, append the line below, and open a pull request.

The first two entries were committed on 2026-07-02 to a predecessor repository
that is private, so their `anchor:` commits resolve there and not here. The
chain continues from those entries: the next digest anchors to this file's
first merge commit in this repository.


| date (UTC) | digest (sha256 of audit tables) | rows | note |
| --- | --- | --- | --- |
| 2026-07-02 | `c845263aba4a4e529fed16198eedbc07eab1cf30c1f0fc46ad893c14e29f7915` | file=30 grants=2 cites=45 sessions=0 plates=0 sales=0 | first digest — Ohio Vol. I sources/rights backfill (OSM ODbL, census PD, us-states flagged unverified) |
| 2026-07-02 | `72a2da4a8265eb2d507c47db1ac8ffc4f1a2a093995f20aed63938ee3612c065` | file=31 grants=3 cites=45 sessions=0 plates=0 sales=0 | us-states → Census cb_2024_us_state_5m (cities#8); boundaries cites moved; `ledger alerts` clean, all 15 pieces. anchor: `e403e62` |
