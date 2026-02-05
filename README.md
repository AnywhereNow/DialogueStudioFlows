# AnywhereNow Dialogue Studio — Sample Flows

A curated set of **ready-to-use example flows** for [AnywhereNow Dialogue Studio]. Use these as blueprints for common integrations, routing patterns, analytics, and diagnostics.

---

## Contents

| Folder | What it demonstrates |
|-------|-----------------------|
| `CustomCRMintegration/` | Patterns for integrating a **custom CRM** (create/search/update entities, case logging, handoff). |
| `DefaultUCCsimple_solution/` | Minimal **UCC** setup; a baseline flow to start a new project quickly. |
| `DynamicsOnlineintegration/` | **Microsoft Dynamics 365** online: auth, contact/case creation, activity logging. |
| `DynamicsPutTranscriptandRecordinginActivity/` | Attach **call transcripts and recording links** to a Dynamics activity. |
| `EventBusUCCEnricher/` | Attach **uccName** to events that don't have them. | 
| `GenericDialogueProviderTemplate/` | A **kickstart blueprint** for integrating with the AnywhereNow Generic Dialogue Provider (GDP) from Dialogue Studio. |
| `HistoryACDC/` | Examples around **ACD** history and callback/continuity patterns. |
| `QMMonitorQuestion/` | Capturing **Quality Monitoring (QM)** inputs for later analysis. |
| `RetentionPolicy/` | The Retention Policy Flow to get information from the Retention Policy List in your Sharepoint UCC settings page |
| `Salesforceintegration/` | **Salesforce**: auth + common object ops (Contact/Case/Task). |
| `SentimentAnalysisAzureBasic/` | **Azure Cognitive Services** sentiment scoring + branching. |
| `TranscriptTodebug_minimal/` | Smallest **transcription debug** flow for troubleshooting STT/latency. |
| `TutorialBase1/` | Starter **tutorial** scaffolding: recommended nodes, wiring patterns, and comments. |
| `UsefulSamples/` | Reusable **snippets** (utility functions, error handlers, timers, helpers). |
| `VoiceForwardToCoworker/` | **Forward voice** to a colleague with presence checks and fallbacks. |
| `webagentCustomCrm/` | WebAgent + **custom CRM** interaction patterns (open, screen-pop, search). |

> Tip: Each folder’s flow(s) can be used as-is or cherry-picked into your existing projects.

---

## Quick start

### Option A — Import a JSON flow
1. Open your Dialogue Studio environment.
2. Press **`Ctrl + i`** (or **Menu → Import**) and paste or upload the JSON from a sample folder.
3. Review any **Function** or **Configuration** nodes and fill in required values (URLs, keys).
4. Click **Deploy** and test.

### Option B — Connect Dialogue Studio to a remote Git
If you prefer to work with version control:
1. Create a Git repository in your Git hosting (e.g., Azure DevOps).
2. Follow the **Remote Git** setup for Dialogue Studio (clone URL, credentials).
3. Pull this repository’s contents (or copy selected sample folders) into your remote.
4. Use the **Commit**/**Push**/**Pull** workflow inside Dialogue Studio to manage changes.

---

## Prerequisites

- An active **AnywhereNow Dialogue Studio** instance with access to the necessary platform services (UCC, connectors, Event Bus).
- For cloud integrations (e.g., **Azure Cognitive Services**, **Microsoft Graph**, **Dynamics 365**, **Salesforce**), ensure credentials, app registrations, and any allow-listing are in place.
- Database samples require a reachable SQL instance and appropriate credentials.

---

## Configure & run

1. **Open the sample flow** and locate the **Configuration**/**Function** nodes.
2. **Set secrets & endpoints** (keys, base URLs, tenant IDs, queue/skill names, etc.).
3. **Adapt routing** to your skills/UCC names and business rules.
4. **Test the happy path**, then try common error paths (timeouts, 4xx/5xx, auth failures).
5. **Log & observe**: most samples include debug nodes—leave these on during initial testing.

---

## Compatibility

This repo can include **outdated** flows. While we try to keep them current, **some samples may lag behind platform changes**.

- If you spot something broken or outdated, please **open an Issue** with details, or **submit a PR** with a fix:
  - Issues: https://github.com/AnywhereNow/DialogueStudioFlows/issues/new/choose
  - Pull Requests: https://github.com/AnywhereNow/DialogueStudioFlows/compare

Your feedback helps us keep these examples useful.

---

## Contributing

We welcome improvements and new examples!

1. **Fork** the repo and create a **feature branch**.
2. Include a short **README.md** in your sample’s folder describing what it does, required config, and a quick test plan.
3. Open a **Pull Request** with screenshots (if relevant) and a brief rationale.

For bugs or requests, open an **Issue** with:
- The sample folder name
- Steps to reproduce
- Expected vs. actual behavior
- Dialogue Studio & connector versions

---

## License & support

Samples are provided as educational examples. Check this repository’s License file (or your customer agreement) for permitted usage. Need help implementing a pattern in production? Contact your AnywhereNow representative.

---

## Useful links

- **Dialogue Studio — Overview**  
  https://golive.anywhere.now/platform_elements/dialogue_studio/dialogue-studio-overview.html

- **Dialogue Studio — User Guide**  
  https://golive.anywhere.now/platform_elements/dialogue_studio/dialogue-studio-user-guide.html

- **Dialogue Studio — Core Nodes**  
  https://golive.anywhere.now/platform_elements/dialogue_studio/dialogue-studio-nodes.html

- **Dialogue Studio — Dialogue Manager Nodes**  
  https://golive.anywhere.now/platform_elements/dialogue_studio/dialogue-studio-dialogue-manager-nodes.html

- **Dialogue Studio — Additional Configuration**  
  https://golive.anywhere.now/platform_elements/dialogue_studio/dialogue-studio-additional-configuration.html

- **How to set up Remote Git (Azure DevOps)**  
  https://golive.anywhere.now/platform_elements/dialogue_studio/additionalconfiguration/dialogue-studio-setting-up-remote-git.html

- **Dialogue Studio — Installation**  
  https://golive.anywhere.now/platform_elements/dialogue_studio/dialogue-studio-install-manual.html

- **Dialogue Studio — FAQ**  
  https://golive.anywhere.now/faq/faq_dialogue_studio.html
