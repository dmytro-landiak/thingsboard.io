# TBMQ Documentation Improvement Plan

> **For agentic workers:** This plan is executed section-by-section with user approval gates. Within each section, dispatch one sub-agent per guide (cap 5 concurrent) using the per-guide brief in the spec. Mark a checkbox `[x]` only after the sub-agent's report has been reviewed.

**Goal:** Improve every in-scope TBMQ doc page (~72 guides) for grammar, technical correctness against TBMQ source repos, MQTT-spec accuracy, command executability, and diagram coverage.

**Spec:** `docs/superpowers/specs/2026-05-25-tbmq-docs-improvement-design.md`

**Tech Stack:** Astro + Starlight; MDX content collections; shared `_includes/` pattern.

---

## Status legend

- `[ ]` — not started
- `[~]` — in progress (e.g. sub-agent dispatched but not yet reported back; or report received but pending review)
- `[x]` — done and reviewed

## Section status overview

| # | Section | Status | Done / Total |
|---|---|---|---|
| 1 | Getting Started: Welcome & Core concepts | done | 9 / 9 |
| 2 | Guides: Security | not started | 0 / 13 |
| 3 | Guides: MQTT essentials | not started | 0 / 10 |
| 4 | Guides: Integration with ThingsBoard | not started | 0 / 1 |
| 5 | Guides: Broker operations | not started | 0 / 7 |
| 6 | Guides: Integrations | not started | 0 / 4 |
| 7 | Guides: Management console / UI | not started | 0 / 9 |
| 8 | Guides: White Labeling & Subscription (PE-only) | not started | 0 / 3 |
| 9 | Reference: Architecture | not started | 0 / 4 |
| 10 | Reference: Performance tests | not started | 0 / 3 |
| 11 | Reference: REST APIs | not started | 0 / 4 |
| 12 | Releases & Support | not started | 0 / 4 |
| 13 | Guides landing | not started | 0 / 1 |
| | **Total** | | **9 / 72** |

Phase 3 — Final synthesis: `tbmq-docs-future-work.md` (root). Status: pending.

---

## Path conventions

All paths in this plan are relative to the repo root `/home/dlandiak/projects/thingsboard.io/`.

- Include base: `src/content/_includes/docs/mqtt-broker/`
- CE stub base: `src/content/docs/docs/mqtt-broker/`
- PE stub base: `src/content/docs/docs/mqtt-broker/pe/`

Each guide row lists: include · CE stub · PE stub (or `—` if absent).

---

## Section 1 — Getting Started: Welcome & Core concepts (0/9)

- [x] **G1.1** `index.mdx` · CE: `index.mdx` · PE: `pe/index.mdx`
- [x] **G1.2** `why-tbmq.mdx` · CE: `why-tbmq.mdx` · PE: `pe/why-tbmq.mdx`
- [x] **G1.3** `getting-started.mdx` · CE: `getting-started.mdx` · PE: `pe/getting-started.mdx`
- [x] **G1.4** `concepts/client-types.mdx` · CE: `concepts/client-types.mdx` · PE: `pe/concepts/client-types.mdx`
- [x] **G1.5** `concepts/sessions.mdx` · CE: `concepts/sessions.mdx` · PE: `pe/concepts/sessions.mdx`
- [x] **G1.6** `concepts/topics.mdx` · CE: `concepts/topics.mdx` · PE: `pe/concepts/topics.mdx`
- [x] **G1.7** `concepts/qos.mdx` · CE: `concepts/qos.mdx` · PE: `pe/concepts/qos.mdx`
- [x] **G1.8** `concepts/security.mdx` · CE: `concepts/security.mdx` · PE: `pe/concepts/security.mdx`
- [x] **G1.9** `concepts/clustering.mdx` · CE: `concepts/clustering.mdx` · PE: `pe/concepts/clustering.mdx`

## Section 2 — Guides: Security (0/13)

- [ ] **G2.1** `security/overview.mdx` · CE: `security/overview.mdx` · PE: `pe/security/overview.mdx`
- [ ] **G2.2** `security/mqtts.mdx` · CE: `security/mqtts.mdx` · PE: `pe/security/mqtts.mdx`
- [ ] **G2.3** `security/enable-https.mdx` · CE: `security/https.mdx` · PE: `pe/security/https.mdx`
- [ ] **G2.4** `security/listeners.mdx` · CE: `security/listeners.mdx` · PE: `pe/security/listeners.mdx`
- [ ] **G2.5** `security/authentication/basic.mdx` · CE: `security/authentication/basic.mdx` · PE: `pe/security/authentication/basic.mdx`
- [ ] **G2.6** `security/authentication/x509.mdx` · CE: `security/authentication/x509.mdx` · PE: `pe/security/authentication/x509.mdx`
- [ ] **G2.7** `security/authentication/jwt.mdx` · CE: `security/authentication/jwt.mdx` · PE: `pe/security/authentication/jwt.mdx`
- [ ] **G2.8** `security/authentication/scram.mdx` · CE: `security/authentication/scram.mdx` · PE: `pe/security/authentication/scram.mdx`
- [ ] **G2.9** `security/authentication/http.mdx` · CE: `security/authentication/http.mdx` · PE: `pe/security/authentication/http.mdx`
- [ ] **G2.10** `security/oauth-2-support.mdx` **(PE)** · CE: — · PE: `pe/security/oauth-2-support.mdx`
- [ ] **G2.11** `security/domains.mdx` **(PE)** · CE: — · PE: `pe/security/domains.mdx`
- [ ] **G2.12** `security/rbac.mdx` **(PE)** · CE: — · PE: `pe/security/rbac.mdx`
- [ ] **G2.13** `security/audit-log.mdx` **(PE)** · CE: — · PE: `pe/security/audit-log.mdx`

## Section 3 — Guides: MQTT essentials (0/10)

- [ ] **G3.1** `user-guide/mqtt-protocol.mdx` · CE: `user-guide/mqtt-protocol.mdx` · PE: `pe/user-guide/mqtt-protocol.mdx`
- [ ] **G3.2** `user-guide/mqtt-broker.mdx` · CE: `user-guide/mqtt-broker.mdx` · PE: `pe/user-guide/mqtt-broker.mdx`
- [ ] **G3.3** `user-guide/topics.mdx` · CE: `user-guide/topics.mdx` · PE: `pe/user-guide/topics.mdx`
- [ ] **G3.4** `user-guide/qos.mdx` · CE: `user-guide/qos.mdx` · PE: `pe/user-guide/qos.mdx`
- [ ] **G3.5** `user-guide/clean-persistent-sessions.mdx` · CE: `user-guide/clean-persistent-sessions.mdx` · PE: `pe/user-guide/clean-persistent-sessions.mdx`
- [ ] **G3.6** `user-guide/mqtt-over-ws.mdx` · CE: `user-guide/mqtt-over-ws.mdx` · PE: `pe/user-guide/mqtt-over-ws.mdx`
- [ ] **G3.7** `user-guide/shared-subscriptions.mdx` · CE: `user-guide/shared-subscriptions.mdx` · PE: `pe/user-guide/shared-subscriptions.mdx`
- [ ] **G3.8** `user-guide/retained-messages.mdx` · CE: `user-guide/retained-messages.mdx` · PE: `pe/user-guide/retained-messages.mdx`
- [ ] **G3.9** `user-guide/last-will.mdx` · CE: `user-guide/last-will.mdx` · PE: `pe/user-guide/last-will.mdx`
- [ ] **G3.10** `user-guide/keep-alive.mdx` · CE: `user-guide/keep-alive.mdx` · PE: `pe/user-guide/keep-alive.mdx`

## Section 4 — Guides: Integration with ThingsBoard (0/1)

- [ ] **G4.1** `user-guide/integration-with-thingsboard.mdx` · CE: `user-guide/integrations/how-to-connect-thingsboard-to-tbmq.mdx` · PE: `pe/user-guide/integrations/how-to-connect-thingsboard-to-tbmq.mdx`

## Section 5 — Guides: Broker operations (0/7)

- [ ] **G5.1** `user-guide/mqtt-client-type.mdx` · CE: `user-guide/mqtt-client-type.mdx` · PE: `pe/user-guide/mqtt-client-type.mdx`
- [ ] **G5.2** `user-guide/blocked-clients.mdx` · CE: `other/blocked-client.mdx` · PE: `pe/other/blocked-client.mdx`
- [ ] **G5.3** `user-guide/backpressure.mdx` · CE: `user-guide/backpressure.mdx` · PE: `pe/user-guide/backpressure.mdx`
- [ ] **G5.4** `user-guide/msg-delivery-strategies.mdx` · CE: `other/msg-delivery-strategy.mdx` · PE: `pe/other/msg-delivery-strategy.mdx`
- [ ] **G5.5** `user-guide/proxy-protocol.mdx` · CE: `other/proxy-protocol.mdx` · PE: `pe/other/proxy-protocol.mdx`
- [ ] **G5.6** `user-guide/health-api.mdx` · CE: `other/health.mdx` · PE: `pe/other/health.mdx`
- [ ] **G5.7** `user-guide/bulk-provisioning.mdx` · CE: `other/bulk-provisioning.mdx` · PE: `pe/other/bulk-provisioning.mdx`

## Section 6 — Guides: Integrations (0/4)

- [ ] **G6.1** `integrations.mdx` (landing) · CE: `integrations.mdx` · PE: `pe/integrations.mdx`
- [ ] **G6.2** `integrations/http.mdx` · CE: `integrations/http.mdx` · PE: `pe/integrations/http.mdx`
- [ ] **G6.3** `integrations/mqtt.mdx` · CE: `integrations/mqtt.mdx` · PE: `pe/integrations/mqtt.mdx`
- [ ] **G6.4** `integrations/kafka.mdx` · CE: `integrations/kafka.mdx` · PE: `pe/integrations/kafka.mdx`

## Section 7 — Guides: Management console / UI (0/9)

- [ ] **G7.1** `user-guide/ui/monitoring.mdx` · CE: `user-guide/ui/monitoring.mdx` · PE: `pe/user-guide/ui/monitoring.mdx`
- [ ] **G7.2** `user-guide/ui/sessions.mdx` · CE: `user-guide/ui/sessions.mdx` · PE: `pe/user-guide/ui/sessions.mdx`
- [ ] **G7.3** `user-guide/ui/subscriptions.mdx` · CE: `user-guide/ui/subscriptions.mdx` · PE: `pe/user-guide/ui/subscriptions.mdx`
- [ ] **G7.4** `user-guide/ui/mqtt-client-credentials.mdx` · CE: `user-guide/ui/mqtt-client-credentials.mdx` · PE: `pe/user-guide/ui/mqtt-client-credentials.mdx`
- [ ] **G7.5** `user-guide/ui/unauthorized-clients.mdx` · CE: `user-guide/ui/unauthorized-clients.mdx` · PE: `pe/user-guide/ui/unauthorized-clients.mdx`
- [ ] **G7.6** `user-guide/ui/websocket-client.mdx` · CE: `user-guide/ui/websocket-client.mdx` · PE: `pe/user-guide/ui/websocket-client.mdx`
- [ ] **G7.7** `user-guide/ui/application-shared-subscriptions.mdx` · CE: `user-guide/ui/shared-subscriptions.mdx` · PE: `pe/user-guide/ui/shared-subscriptions.mdx`
- [ ] **G7.8** `user-guide/ui/users.mdx` · CE: `user-guide/ui/users.mdx` · PE: `pe/user-guide/ui/users.mdx`
- [ ] **G7.9** `user-guide/ui/settings.mdx` · CE: `user-guide/ui/settings.mdx` · PE: `pe/user-guide/ui/settings.mdx`

## Section 8 — Guides: White Labeling & Subscription (PE-only) (0/3)

- [ ] **G8.1** `white-labeling.mdx` **(PE)** · CE: — · PE: `pe/white-labeling.mdx`
- [ ] **G8.2** `white-labeling/image-gallery.mdx` **(PE)** · CE: — · PE: `pe/image-gallery.mdx`
- [ ] **G8.3** `user-guide/private-cloud-subscription.mdx` **(PE)** · CE: — · PE: `pe/subscription.mdx`

## Section 9 — Reference: Architecture (0/4)

- [ ] **G9.1** `architecture.mdx` · CE: `architecture.mdx` · PE: `pe/architecture.mdx`
- [ ] **G9.2** `reference/architecture/persistent-device-client.mdx` · CE: `architecture-details/persistent-device-client.mdx` · PE: `pe/architecture-details/persistent-device-client.mdx`
- [ ] **G9.3** `reference/architecture/persistent-application-client.mdx` · CE: `architecture-details/persistent-app-client.mdx` · PE: `pe/architecture-details/persistent-app-client.mdx`
- [ ] **G9.4** `reference.mdx` (landing) · CE: `reference.mdx` · PE: `pe/reference.mdx`

## Section 10 — Reference: Performance tests (0/3)

- [ ] **G10.1** `reference/1m-throughput-p2p-performance-test.mdx` · CE: `reference/1m-throughput-p2p-performance-test.mdx` · PE: `pe/reference/1m-throughput-p2p-performance-test.mdx`
- [ ] **G10.2** `reference/3m-throughput-single-node-performance-test.mdx` · CE: `reference/3m-throughput-single-node-performance-test.mdx` · PE: `pe/reference/3m-throughput-single-node-performance-test.mdx`
- [ ] **G10.3** `reference/100m-connections-performance-test.mdx` · CE: `reference/100m-connections-performance-test.mdx` · PE: `pe/reference/100m-connections-performance-test.mdx`

## Section 11 — Reference: REST APIs (0/4)

- [ ] **G11.1** `rest-api.mdx` (landing) · CE: `rest-api.mdx` · PE: `pe/rest-api.mdx`
- [ ] **G11.2** `reference/rest-api/user-management.mdx` · CE: `user-management.mdx` · PE: `pe/user-management.mdx`
- [ ] **G11.3** `reference/rest-api/mqtt-client-credentials-management.mdx` · CE: `mqtt-client-credentials-management.mdx` · PE: `pe/mqtt-client-credentials-management.mdx`
- [ ] **G11.4** `reference/rest-api/application-shared-subscriptions-management.mdx` · CE: `application-shared-subscription.mdx` · PE: `pe/application-shared-subscription.mdx`

## Section 12 — Releases & Support (0/4)

- [ ] **G12.1** `changelog.mdx` (Releases & roadmap landing) · CE: `changelog.mdx` · PE: `pe/changelog.mdx`
- [ ] **G12.2** `releases.mdx` · CE: `releases.mdx` · PE: `pe/releases.mdx`
- [ ] **G12.3** `roadmap.mdx` · CE: `roadmap.mdx` · PE: `pe/roadmap.mdx`
- [ ] **G12.4** `help.mdx` · CE: `help.mdx` · PE: `pe/help.mdx`

## Section 13 — Guides landing (0/1)

- [ ] **G13.1** `user-guide.mdx` (Guides landing — card grid) · CE: `user-guide.mdx` · PE: `pe/user-guide.mdx`

---

## Phase 3 — Final synthesis

- [ ] Write `tbmq-docs-future-work.md` at repo root with P0/P1/P2 prioritization covering:
  - Gaps in current docs — guides that should exist but don't.
  - MQTT-related additions — spec deep-dives, v5 feature explainers, interoperability notes.
  - TBMQ-specific additions — clustering internals, perf-tuning cookbook, DR playbook, integration recipes, observability/alerting rules.
  - Cross-product additions — TBMQ ↔ ThingsBoard platform, TBMQ ↔ Edge, TBMQ ↔ Kafka bridge patterns.

---

## Per-section progress reports

(Appended after each section finishes. Each entry lists, for every guide in the section: file, change counts by category, any could-not-verify items, and any open questions for the user.)

### Section 1 — Getting Started

Repo refs at start: TBMQ CE `~/projects/tbmq` `develop/2.4` @ `a2d88dd56`; TBMQ PE `~/projects/tbmq-pe` `develop/2.4` @ `c847299f2`. Diff: 9 includes touched, +543/-244 lines; no stubs modified.

| Guide | Grammar | Tech | MQTT | Cmd | Diagrams | Could-not-verify | Open Qs |
|---|---|---|---|---|---|---|---|
| G1.1 `index.mdx` | 3 | 0 | 0 | 0 | 0 | none | "Connect in minutes" SplitCard could embed `<LiveDemoCard />` for SSOT — held off (visual balance / design review needed) |
| G1.2 `why-tbmq.mdx` | 9 | 4 | 1 (§3.3, §3.4) | 0 | 3 | none | Legacy MQTT 3.1 link points to fragile IBM developerWorks host — consider durable URL |
| G1.3 `getting-started.mdx` | 19 | 1 | 0 | 0 | 1 | `pnpm check` not run (node_modules missing) | Env var `SECURITY_MQTT_BASIC_ENABLED=true` still in bundled docker-compose / k8s but no longer read by Java code — cleanup out of scope |
| G1.4 `concepts/client-types.mdx` | 4 | 3 | 0 | 0 | 1 | `pnpm check` not run (node_modules missing) | `ClientType` enum also has `INTEGRATION` — internal use, not exposed via credentials. Add a footnote? |
| G1.5 `concepts/sessions.mdx` | 6 | 3 | 1 (5.0 §3.1.2.11.2, §4.1) | 0 | 1 | none | Operational TTL detail in this conceptual page — move to user-guide/clean-persistent-sessions instead? |
| G1.6 `concepts/topics.mdx` | 6 | 4 | 2 (5.0 §1.5.4, §4.7.1.3) | 0 | 2 | none | Aside suggesting `MQTT_TOPIC_MAX_SEGMENTS_COUNT=5–10` is editorial, not from any source — confirm guidance number or loosen wording |
| G1.7 `concepts/qos.mdx` | 9 | 5 | 3 (3.1.1 §3.6 §4.3.3 §4.4, 5.0 §3.6 §4.4 §3.9.3) | 0 | 2 | none | none |
| G1.8 `concepts/security.mdx` | 12 | 5 | 3 (5.0 §3.15 §3.4.2.1 §3.5.2.1 §3.9.3 §3.2.2.2, 3.1.1 §3.9.3 §3.2.2.3) | 0 | 1 | none | none |
| G1.9 `concepts/clustering.mdx` | 9 | 3 | 0 (cited 3.1.1 §3.3.1, §4.4 / 5.0 §4.4, §4.8.2 for reference) | 0 | 1 | none | Dead `import { Products }` mirrors siblings — strip across all concept pages? Optional "Shared subs in a cluster" subsection — flagged, not added |

**Totals:** Grammar/clarity edits: 77 · Technical fixes: 28 · MQTT spec fixes: 10 · Command fixes: 0 · Diagram placeholders added: 12

**Cross-section themes for the user:**

1. **Dead `import { Products }` in concept page MDX.** G1.9 noted this — `Products` is imported but only `props.product` is used. All six concept pages share the pattern. Consider a follow-up cleanup PR (out of scope here).
2. **Legacy MQTT 3.1 reference link** in G1.2 points to an IBM developerWorks draft (fragile host). Worth flagging for a more durable canonical URL.
3. **Stale env var `SECURITY_MQTT_BASIC_ENABLED`** in bundled docker-compose / k8s manifests but not read by current Java code (G1.3). Out-of-scope cleanup item.
4. **`ClientType.INTEGRATION`** exists in the enum but is internal-only — not exposed via MQTT credentials (G1.4). Add a one-line footnote? Decision deferred.
5. **No stubs were edited.** Every change landed in the shared include only, so CE and PE see the same content (as the spec requires).
6. **No commands needed correction in this section.** All `mosquitto_pub/sub`, install script, docker-compose, env-var, and topic-name strings were preserved verbatim and verified against TBMQ source.

### Section 2 — Security
_(pending)_

### Section 3 — MQTT essentials
_(pending)_

### Section 4 — Integration with ThingsBoard
_(pending)_

### Section 5 — Broker operations
_(pending)_

### Section 6 — Integrations
_(pending)_

### Section 7 — Management console / UI
_(pending)_

### Section 8 — White Labeling & Subscription (PE-only)
_(pending)_

### Section 9 — Reference: Architecture
_(pending)_

### Section 10 — Reference: Performance tests
_(pending)_

### Section 11 — Reference: REST APIs
_(pending)_

### Section 12 — Releases & Support
_(pending)_

### Section 13 — Guides landing
_(pending)_

---

## Resumption checklist

To continue work in a new session:

1. Read this plan top to bottom.
2. Find the first section with unchecked boxes. If any box is `[~]`, that's the section currently in progress — finish reviewing those sub-agent reports first.
3. Confirm with the user: "Continue Section N: <name>?" Wait for explicit "go".
4. Dispatch one sub-agent per pending guide in that section, cap 5 concurrent. Use the per-guide brief in the spec.
5. As each report comes back, mark `[x]` and add a one-line note in the per-section progress report below.
6. When the section completes, post the per-guide summary table to the user and ask which section to do next.
