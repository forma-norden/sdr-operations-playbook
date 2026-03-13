# Ecosystem: sdr-operations-playbook

How this repo connects to the rest of the Forma Norden GTM library.

## Works With

| Repo | Relationship | When to use together |
|------|-------------|---------------------|
| ``gtm-plays-collection`` | Upstream | SDRs execute the plays defined in the plays collection using the workflows defined here. |
| ``cold-email-copy-playbook`` | Parallel | The copy framework rules defined here dictate how the templates in the copy playbook are customized. |
| ``outbound-personalization-playbook`` | Upstream | Research frameworks from that playbook feed directly into the execution blocks defined in this playbook. |
| ``linkedin-profile-dm-conversion-playbook`` | Parallel | Extends the multi-channel approach from email/call into social selling. |

## Suggested Skill Chains

1. The Complete Outbound Setup: ``sdr-daily-workflow-operator`` (set the schedule) > ``personalization-research-framework`` (do the research) > ``sdr-cold-call-scripts`` + ``sdr-outbound-writing-rules`` (execute the outreach).
2. Fixing SDR Performance: ``sdr-metrics-benchmarks`` (find the leak) > ``sdr-prompt-library`` (build tools to fix it).
