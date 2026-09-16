# MathWise DI² — Erdős 125 Primal-Anchored Rotation-Branch Root Isolation

This repository preserves a compact audit packet for a 37-variable rational polynomial system associated with a fixed Erdős Problem 125 branch.

## Recorded result

The packet records:

- a 430-digit numerical root;
- a rational center rounded to 120 decimal places;
- a common box radius of `1e-100`;
- a rational approximate inverse rounded to 100 decimal places;
- exact rational Krawczyk bounds with strict inclusion;
- Jacobian rank `37` and a positive minimum singular value; and
- a conditional objective interval.

`rotation_root_isolation.json` records `candidate_sha256_match: true`, a scaled 430-digit root residual of approximately `2.01e-430`, and the packet input hash `50817a80ec3e13832e682e2215c2d511458542101d21ce8474eac0e6ba6489a1`.

## Evidence and provenance

The source system is in `rotation_polynomial_system.txt`; numerical data are preserved in `rotation_root_430digits.txt`, `center_120dp.tsv`, and `approx_inverse_A_100dp.tsv`. `SHA256SUMS.txt` verifies the six listed files in this checkout.

## Scope and limitations

This is a fixed root-isolation packet, not a complete solution to Erdős Problem 125. The packet itself states that it does not contain or claim an exact K-completion or global coercivity certificate. No standalone replay executable is included, so a fresh independent reproduction is **UNVERIFIED** from this repository alone. The result also depends on the stated variable order, rational system, floating-point source fields, and declared symmetry handling.

## How to review

Start with [`README.txt`](README.txt), then inspect `rotation_root_isolation.json`, the polynomial system, the center/inverse tables, and the checksum file. Do not infer global theorem status from this local root-isolation record.

Publisher: Grounded DI LLC
