# Session Handoff

## Verified Now

- What is currently working: the five-subsystem harness, the OpenSpec integration, the verification gate, and the CI workflow.
- What verification actually ran: `./init.sh`, `node scripts/validate-harness.mjs`, and `openspec validate --all --strict`.

## Changed This Session

- Code or behavior added: none — this is a template-only repository.
- Infrastructure or harness changes: created the template structure, scripts, documentation, and OpenSpec configuration.

## Broken Or Unverified

- Known defect: none.
- Unverified path: project-specific install, test, and start commands are auto-detected and have not been exercised because the template has no application code.
- Risk for the next session: replacing the template-maintenance features without updating `feature_list.json` evidence will fail the harness validator.

## Next Best Step

- Highest-priority unfinished feature: none in the template; adopters should add their first product feature.
- Why it is next: the template is complete and verified; the next useful step is project adoption.
- What counts as passing: `./init.sh` passes with the adopter's commands and the new feature has recorded evidence.
- What must not change during that step: the five subsystem files and the verification contract.

## Commands

- Startup: `./init.sh`
- Verification: `./scripts/verify.sh`
- Focused debug command: `node scripts/validate-harness.mjs`
