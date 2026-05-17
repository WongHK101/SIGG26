# Current Provenance Files - 2026-05-17

This directory contains the current machine-readable evidence used by the manuscript.

## Files

- `table3_depth_provenance.json`: source mapping for the current validation-gated reference-depth table.
- `table3_depth_scene_stats.csv`: scene-level depth stats used by the supplement.
- `table3_depth_scene_stats.json`: JSON form of scene-level depth stats.
- `figure2_depth_provenance.json`: source mapping for the current main depth figure.
- `table6_support_audit_quantitative.csv`: quantitative support-audit evidence.
- `table6_support_audit_quantitative.json`: JSON form of the support-audit evidence.
- `umgs_i_direct_support_audit_20260517.csv`: direct UMGS-I four-scene, per-band support audit.
- `umgs_i_direct_support_audit_20260517.json`: JSON form of the UMGS-I direct support audit.
- `product_coverage_by_scene_method_index_20260517.csv`: product-level common-support coverage by scene, method, and vegetation index.
- `product_coverage_summary_20260517.json`: JSON summary for the product-coverage diagnostic.
- `raw_conditioning_ablation_three_scene_20260517.csv`: three-scene no-valid-mask ablation summary used by Table~\ref{tab:raw-conditioning-ablation}.
- `raw_conditioning_ablation_three_scene_20260517.json`: JSON form of the three-scene no-valid-mask ablation summary.
- `raw_conditioning_ablation_audits_20260517/`: per-scene no-valid-mask training-protocol audits, support audits, comparison CSV/JSON, and run event logs.

## Current Source Bundle

The active data source is:

- `E:\paper\SIGS\data\d_20260511`

Current depth summary entrypoint:

- `E:\paper\SIGS\data\d_20260511\02_depth_valid\summary_current_4scene_20260512`

## Audit Status

On 2026-05-17, local path references in these provenance files were checked and found present. Remote `/root/...` references extracted from the current handoff/provenance were also checked on AutoDL after restart and found present.

For directly mappable local-vs-AutoDL evidence files, 15 files hash-matched exactly; the only missing mapped item was the local explanatory note `README_COORD_FIX.md`, not an evaluation output.
