# Release Checklist (Template)

Use this checklist to coordinate releases and ensure prescriptive verification and rollback plans are in place.

Pre-release
- [ ] PRs merged and linked to issues with acceptance criteria
- [ ] CI passing (unit, integration), and security scans completed
- [ ] Release Manager has confirmed deployment window
- [ ] Backup / snapshot plan ready (if applicable)
- [ ] Rollback plan documented and tested (if possible)
- [ ] Data & Measurement Lead has instrumentation validated
- [ ] Security sign-off (if required) from Security Liaison
- [ ] SRE/On-call are notified and ready for the window

Staging verification
- [ ] Deploy to staging and run smoke tests
- [ ] Run performance and critical path checks
- [ ] Validate key telemetry and success metrics

Production deployment
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy smoke tests and health checks
- [ ] Monitor dashboards and on-call alerts for first 30-60 minutes
- [ ] Communicate release status to stakeholders (channel + release notes)

Post-release
- [ ] Confirm no critical incidents in monitoring window
- [ ] Log post-release verification results
- [ ] Open action items for any follow-up bugs or improvements
- [ ] Announce release to stakeholders and support teams

Notes:
- Include links to runbooks, rollback procedures, and dashboards in the release PR or release notes.
