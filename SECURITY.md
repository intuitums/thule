# Security Policy

thule is a sandboxing boundary, so its own security matters more than
most projects' — but nothing is implemented yet. There is no released
code, no running guest, and no boundary to test against.

Once a first implementation lands, this document will define what "in
scope" means precisely (guest escape, host filesystem/network reachable
from the guest beyond the mounted workspace, credential leakage into the
guest, and so on) and where to report it.

Until then: if you find a design flaw in how this is being planned — a
proposed mount, exec, or filesystem-bridging approach that wouldn't
actually hold a boundary — open an issue rather than a private report;
there's no live boundary yet for a private disclosure to protect.

## Reporting a vulnerability (once code exists)

Report privately through
[GitHub Security Advisories](https://github.com/intuitums/thule/security/advisories/new)
rather than a public issue.
