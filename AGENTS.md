# AGENTS.md — READ FIRST

All Codex/AI work in this repository must read and follow this file before doing anything else.

This project is for a private home-lab/home-network environment with practical security roughly comparable to a well-run Home Assistant installation. It is not an FBI/CIA/NASA/critical-infrastructure environment. Avoid unnecessary enterprise/government ceremony and overengineering unless a specific risk justifies it.

## Rollback-first, forward-progress
- Establish a usable rollback before risky/destructive/availability-affecting changes.
- Once rollback is verified, prefer forward progress and real-world validation over repeated approval checkpoints.
- Fix forward when failure is bounded, understood, recoverable, and rollback remains intact.
- Roll back when data, credentials, lockout, exposure, or unclear failure makes continued experimentation unsafe.
- Prefer simple, native, reversible solutions.
- Preserve irreplaceable data; isolate destructive tests.

## Preflight / execution
Read this file first, then project-specific docs. Before substantial work, preflight material conflicts, prerequisites, persistence/rollback, resources, and test gaps. Raise only genuinely material questions before implementation. Once work starts, continue through routine recoverable issues until the planned checkpoint. Distinguish tested candidates from deployed/running code and verify real deployment state.

## Resource safety
Use bounded timeouts for long-running commands where practical and monitor the system actually executing them. On critical memory/swap/disk pressure, sustained severe I/O pressure, or prolonged `D`-state, stop only the affected task-owned child/process group where possible, preserve work/rollback, and report rather than automatically rebooting/deploying/committing/pushing.

## Baseline infrastructure before changes
Verify and record applicable host/hardware, VM/CT/device ID and role, hostname, IP/MAC/gateway/bridge, CPU/RAM/swap/disk, mounts, service ports, users/access, application/service paths, Git state, dependencies, known-good behavior, and rollback path. Do not infer facts that can be verified. Update current-state/infrastructure/change notes as facts change.

Private repos may contain internal topology; public repos must sanitize it.

## Secrets
Never commit passwords, private keys, API tokens, cookies/session secrets, recovery codes, VPN private keys/PSKs, or unsanitized secret-bearing backups. Do not weaken authentication/firewall/isolation merely for convenience unless explicitly justified and reversible.

## Publication
Working repos are private by default during infrastructure-specific development. Public releases should be deliberately sanitized exports with reviewed history.

## Project-specific rules
More specific or stricter project rules supplement and take precedence over this common minimum policy.
