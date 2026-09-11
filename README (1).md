# Expanded sequential DNS timing detector v1.3.1

## Locked immediate path

- Candidate: `w64__baseline+regularity+local_change__64fd5af306`
- Window: `64` same-parent-domain events
- Features: `13` causal content-free timing features
- Direct threshold: `216.140237928340`
- Baseline model/feature/threshold changes: **none**

## New slow path

- Evidence reference: benign calibration scores only
- Evidence-start tail probability: `0.05`
- Time decay: `15.0` minutes
- Accumulator threshold: `35.832336055219`
- Threshold rule: benign q99.9, method `higher`
- Final decision: direct exceedance OR accumulator exceedance

## Benign development validation

- Exposure: `5.570712` days
- Locked direct incidents/day: `0.000000`
- Locked direct budget: `0.050000`/day — retained
- Expanded incidents: `1`
- Expanded incidents/day: `0.179510`
- Expanded hard budget: **not enforced**
- Expanded rate role: reported operating trade-off

## Development attack evaluation

- Original detected profiles: `6`
- Expanded detected profiles: `8`
- Newly detected by the sequential path: `['new_s2_evaluation', 's2_second_attempt']`

## Scientific boundary

The current folder attacks, including the S2 0.125/0.25/0.50 boundary series,
are development profiles because they motivated this architecture. After this
extension is frozen, new captures with unseen seeds, payloads and start times
are required for final evaluation.
