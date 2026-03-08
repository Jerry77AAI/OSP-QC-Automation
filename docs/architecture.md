# OSP QC Automation — Architecture Overview
## System Purpose
AI-powered QC pipeline replacing manual Bluebeam PDF review for OSP telecom Construction Drawings (CD) and Permit Drawings (PD) at Essentia Inc.
## Architecture Diagram
```
[Drawing Input] --> [Claude QC Engine] --> [QC Report]
     |                    |                     |
   PDF/DWG         Checklist Skills        Bluebeam Export
   ArcGIS          Hooks/Guardrails        Excel Dashboard
   AutoCAD         Human Review Gate       Manager Summary
```
## Pipeline Stages
### Stage 1 — Ingestion
- Drawing received (PDF, DWG, or ArcGIS export)
- - Metadata extracted: drawing number, revision, engineer
  - - Routed to correct QC skill based on type (CD vs PD)
    - ### Stage 2 — Automated QC
    - - Claude activates appropriate skill from .claude/skills/
      - - Checks drawing against all checklist items
        - - Flags: CRITICAL / MAJOR / MINOR / NOTE
          - - ArcGIS spatial data cross-referenced for GIS items
            - ### Stage 3 — Human Review Gate
            - - QC Manager reviews AI-generated flag report
              - - Accepts, rejects, or modifies flags in Bluebeam
                - - No drawing passes without human sign-off
                  - ### Stage 4 — Feedback Loop
                  - - QC Manager corrections ingested
                    - - Missed items identified and logged in docs/adr/
                      - - Checklist skill weights updated
                        - ### Stage 5 — Reporting
                        - - QC summary generated (Excel + PPTX)
                          - - Metrics: pass rate, common errors, engineer performance
                            - - Stored in docs/reports/
                              - ## Key Design Decisions
                              - - See docs/adr/ for Architecture Decision Records
                                - ## AI Stack
                                - - Claude: Primary QC reasoning, report generation, office automation
                                  - - Grok: Real-time standard lookups, spec research (Phase 2)
                                    - - ESRI AI: Spatial validation evaluation (Phase 2)
                                      - - Autodesk AI: DWG intelligence evaluation (Phase 2)
                                        - ## Team
                                        - See CLAUDE.md root for full team roster and responsibilities.
