# bio-ai-openclaw-skills

Custom OpenClaw skills for nanoparticle vaccine design, gate-based MD audit, and reproducible computational workflow decisions.

## Included skills

- vaccine-design-orchestrator  
  Evaluate new nanoparticle vaccine candidates, redesign computational workflows, define gate criteria, and return Go / Hold / Kill decisions.

- gate-audit  
  Audit AF2 / ESMFold / AF3 / SASA / MD outputs and return Gate 1–4 judgments, failure modes, and next-step recommendations.

## Install

Copy these skills into your OpenClaw workspace:

    mkdir -p <your-workspace>/skills
    cp -R skills/vaccine-design-orchestrator <your-workspace>/skills/
    cp -R skills/gate-audit <your-workspace>/skills/

## Activation

OpenClaw loads eligible workspace skills when a new session starts.  
After adding or editing a skill, start a new OpenClaw session.

## Example prompts

- Evaluate a new antigen-nanoparticle vaccine candidate and return a Go / Hold / Kill decision.
- Audit these AF2, SASA, and 100 ns MD results using Gate 1–4.
- Redesign this computational screening workflow to reduce unnecessary high-cost simulations.

## Repository structure

    skills/
      vaccine-design-orchestrator/
        SKILL.md
      gate-audit/
        SKILL.md

## Notes

- These skills are designed for structured scientific decision support.
- CpHMD and TI/FEP are not treated as default steps.
- Decisions should include gate conditions, failure modes, and next-step recommendations.
