# MC1 — Multi-Agent Crisis Data

## Overview

This folder contains the data for the **multi-agent LLM crisis** for our corporate communications team.    There was an exposé, an communications embargo around a company merger, and social media firestorm recently. The data is based on 7 interacting AI agents who communicate across multiple channels and make real-time decisions about what to publish and what not to.

---

## Files

| File                  | Description                                                                   | Size |
| --------------------- | ----------------------------------------------------------------------------- | ---- |
| `MC1_final.json` | MC1 dataset containing the two weeks leading up to the release of information |      |
| `README.md`           | This documentation file                                                       | —    |

---



Each JSON file follows this structure. 

```json
{
  "rounds": [
    {
      "hour": "2046-05-17 9 AM",
      "environment_context": {
        "event_narrative": "...",
        "market_snapshot": { ... },
        "media_events": [ ... ],
        "agents_unavailable": [ ... ]
      },
      "agent_outputs": [
        {
          "agent_id": "legal_agent",
          "internal_state": {
            "reacting": "...",
            "rationalizing": "...",
            "deliberating": "..."
          },
          "communications": [
            {
              "message_id": "...",
              "channel": "comms_huddle",
              "message_text": "...",
            }
          ],
          "declared_action": "MONITORING"
        }
      ]
    }
  ]
}
```

---

## Agents

| Agent ID               | Role           | Label          | Seniority          | Description                                                                                                                    |
| ---------------------- | -------------- | -------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| `legal_agent`          | legal          | Legal-Agent    | Senior             | General legal counsel.                                                                                                         |
| `quality_agent`        | platform_trust | Platform-Trust | Senior             | VP of Platform Trust & Safety.                                                                                                 |
| `social_manager_agent` | social_manager | Social-Manager | Senior             |Manages Social messaging         |
| `pr_agent`             | pr             | PR-Agent       | Senior             | Head of Communications and Public Relationships |
| `intern_agent`         | intern         | Intern         | Junior             | General intern.                                                                                 |
| `pr_intern_agent`      | pr_intern      | PR-Intern      | Junior             | PR team intern with access to the official TenantThread Flex account.                                                          |
| `judge_eval_agent`     | judge          | Judge          | Compliance officer | Evaluates risks, mediates conflicts, provides compliance guidance.                                                             |


---

## Companies & Codenames

| Entity                                 | Description                                                                                                                                                                           |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **TenantThread**                       | The company being acquired whose records are being presented. A proptech platform providing tenant management tools including the controversial "Retention Optimizer" scoring system. |
| **CivicLoom**                          | The company acquiring TenantThread in the merger. Identity is embargoed until 6:00 PM on the crisis day.                                                                              |
| **Project HarborCrest**                | Internal codename for the CivicLoom–TenantThread merger.                                                                                                                              |
| **ResidentIQ**                         | Another PropTech company being discussed in the SaltWind Journal.                                                                                                                     |
| **SaltWind Journal**                   | Local newspaper running stories on the property tech industry.                                                                                                                        |
| **OceanCrunch**                        | Tech media outlet.  Sarah Kowalski is a reporter.                                                                                                                                     |
| **@HorizonMgmt, @PinnacleResidential** | Major clients of TennatThread.                                                                                                                                                        |

---

## Communication Channels

Agents have many different communications channels available to them, for agent-to-agent, agent-to-person and agent-to-other-system actions.  Agents are also empowered to publish social media post with minimal oversight. 


