# rlv-code — Plans

_Plan file created by DEV_SWEEP_2026-06 (project had none)._

## Opus 4.8 Expansion (2026-06-01)

**Audit snapshot:** 0 P0, 2 P1 (stale hardcoded metrics with no freshness gate; deploy path documented but not wired — `_deploy.py` absent, CNAME present but unconnected). Code-complete single-file static portfolio site.

### Near-term (audit remediation)

- Implement the deploy path (Porkbun FTP or GitHub Pages) so `code.rlv.lol` actually serves; add a pre-deploy freshness checklist for the hardcoded metrics (glazes/temp/proofs/KG counts).
- Fix the stale `project.json` "awaiting git init" (the `.git/` exists).

### Mid-term (capability)

- Set security headers (CSP/X-Frame-Options) at the host on deploy; consider self-hosting the Google Font to drop the third-party request.

### Long-term (vision)

- Auto-refresh the metrics from live telemetry (share the rlv-lol LOC pipeline) so the portfolio numbers never go stale.

### Next 3 concrete actions

1. Wire the deploy path + connect the CNAME.
2. Add a metrics-freshness checklist.
3. Fix the stale project.json metadata.
