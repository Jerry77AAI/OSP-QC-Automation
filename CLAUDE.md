# CLAUDE.md — OSP QC Automation Consortium
## Repo Memory | North Star Document | Last Updated: March 2026

---

## PURPOSE

Automate QC review of Construction Drawings (CD) and Permit Drawings (PD)
for telecom OSP fiber infrastructure at Essentia Inc.

Goal: Replace manual Bluebeam PDF markup with AI-native QC pipeline that:
- Catches errors automatically against checklist
- - Generates audit-ready QC reports
  - - Learns from human corrections (QC Manager feedback loop)
    - - Scales across CD, PD, Fiber/Duct/Drop Schematics, ArcGIS, AutoCAD
     
      - ---

      ## REPO MAP

      src/qc/         -> QC automation engines (CD + PD)
      src/arcgis/     -> ArcGIS spatial validation + schema checks
      src/autocad/    -> AutoCAD DWG layer compliance + template validation
      src/permits/    -> Permit workflow automation
      docs/           -> Architecture overview, ADRs, team runbooks
      .claude/skills/ -> Reusable AI expert modes (QC checklists, workflows)
      .claude/hooks/  -> Automated guardrails (protect sensitive modules)
      checklists/     -> Source QC checklists (ground truth)

      ---

      ## TEAM

      | Role | Responsibility |
      |------|----------------|
      | Principal (Jerry77AAI) | Co-CTO, Project Lead |
      | Claude (Anthropic) | Co-CTO, AI reasoning, Office automation, Code |
      | Grok | Co-CTO, Real-time data, Search, Research |
      | Sr. GIS Administrator | ArcGIS schema authority |
      | QC Manager | QC sign-off, feedback ingestion |
      | Permit Manager | Permit workflow authority |
      | 2x Engineering II | Project engineering |
      | Lead Drafter OSP II | AutoCAD drafting lead |
      | 2x OSP I | Field/drafting support |
      | Permit Admin | Permit submissions |
      | 10x OSP Engineers | Field engineering |
      | Engineering Manager | Engineering oversight |

      ---

      ## RULES

      ### Always
      - Flag errors traceable to specific checklist item (no free-form flags)
      - - Include checklist item ID in every QC finding
        - - Generate human-readable QC summary for QC Manager review
          - - Preserve Bluebeam markup categories as source of truth for corrections
            - - Cross-reference ArcGIS coordinates when validating CD spatial accuracy
             
              - ### Never
              - - Modify ArcGIS schema without Sr. GIS Administrator sign-off
                - - Auto-approve any drawing — human must confirm all QC passes
                  - - Touch billing, auth, or migration modules
                    - - Commit directly to production QC outputs without human review
                      - - Make assumptions about client specs — always reference source document
                       
                        - ### Quality Standards
                        - - CD QC: Must validate against current construction drawing checklist
                          - - PD QC: Must validate against permit drawing checklist + jurisdiction requirements
                            - - ArcGIS: Coordinate tolerance max 0.5ft for OSP fiber routes
                              - - AutoCAD: All layers must comply with Essentia layer standards
                               
                                - ---

                                ## COMMANDS

                                Run CD QC:     Use skill -> .claude/skills/qc-cd-checklist.md
                                Run PD QC:     Use skill -> .claude/skills/qc-pd-checklist.md
                                ArcGIS Check:  Use skill -> .claude/#s kCiLlAlUsD/Ea.rmcdg i— sO-SvPa lQiCd aAtuotro.mmadt
                                iGoenn eCroantseo rRteipuomr
                                t#:#  URseep os kMielmlo r-y>  |. cNloarutdhe /Sstkairl lDso/cqucm-ernetp o|r tL-agsetn eUrpadtaotre.dm:d
                                M
                                a-r-c-h

                                 2#0#2 6A
                                I
                                 -S-T-A
                                C
                                K#
                                #
                                 CPlUaRuPdOeS E

                                  A u-t>o mPartiem aQrCy  rbervaiienw:  orfe aCsoonnsitnrgu,c tcioodne ,D roafwfiincges  d(oCcDs),  aQnCd  lPoegrimci
                                tG rDorka w i n g s   (-P>D )R
                                efaolr- ttiemlee:c osmt aOnSdPa rfdisb elro oiknufpr,a scturrurcetnutr es paetc sE,s sreensteiaar cIhn
                                cE.S
                                R
                                IG oAaIl :   R e-p>l aEcvea lmuaantuianlg :B lsupeabteiaaml  PvDaFl imdaartkiuopn  wiintthe gArIa-tniaotni v(eP hQaCs ep i2p)e
                                lAiunteo dtehsakt :A
                                I-  -C>a tEcvhaelsu aetrirnogr:s  DaWuGt oimnatteilclailgleyn caeg aiinntsetg rcahteicoknl i(sPth
                                a-s eG e2n)e
                                r
                                a-t-e-s

                                 a#u#d iCtU-RrReEaNdTy  PQHCA SrEe
                                p
                                oPrhtass
                                e-  1L e— aFronusn dfartoimo nh u(mAacnt icvoer)r
                                e-c tRieopnoss i(tQoCr yM asntarguecrt ufreee debsatcakb lliosohpe)d

                                --  SCcLaAlUeDsE .amcdr owsrsi tCtDe,n
                                P-D ,F iFrisbte rs/kDiulclts/ Dbreoipn gS cbhueimlatt
                                i-c sN,e xAtr:c GCIDS ,Q CA uatuotCoAmDa
                                t
                                i-o-n-
                                e
                                n#g#i nReE
                                P
                                O- -M-A
                                P

                                #
                                #s rFcE/EqDcB/A C K   L O O P

                                 -W>h eQnC  QaCu tMoamnaatgieorn  pernogviindeess  (mCaDr k+e dP-Du)p
                                 scrocr/raercctgiiosn/s :
                                 1 .  -I>n gAersctG ImSa rskpuapt icaalt evgaolriideast iforno m+  Bslcuheebmeaa mc heexcpkosr
                                ts
                                r2c./ aCuotmopcaarde/  a g a i-n>s tA uAtIo CQACD  fDlWaGg sl
                                a3y.e rI dceonmtpilfiya nmcies s+e dt eimtpelmast e- >v aulpiddaattei ocnh
                                escrkcl/ipsetr msiktisl/l
                                 4 .  -L>o gP ecromrirte cwtoiroknf lionw  daouctso/maadtri/o na
                                sd odcesc/i s i o n   r e c o r d-
                                >5 .A rRcehtirtaeicnt ucrhee cokvleirsvti ewwe,i gAhDtRisn,g  taecacmo rrduinnbgoloyks
                                >.claude/skills/ -> Reusable AI expert modes (QC checklists, workflows)
                                >.claude/hooks/  -> Automated guardrails (protect sensitive modules)
                                >checklists/     -> Source QC checklists (ground truth)
                                >
                                >---
                                >
                                >## TEAM
                                >
                                >| Role | Responsibility |
                                >|------|----------------|
                                >| Principal (Jerry77AAI) | Co-CTO, Project Lead |
                                >| Claude (Anthropic) | Co-CTO, AI reasoning, Office automation, Code |
                                >| Grok | Co-CTO, Real-time data, Search, Research |
                                >| Sr. GIS Administrator | ArcGIS schema authority |
                                >| QC Manager | QC sign-off, feedback ingestion |
                                >| Permit Manager | Permit workflow authority |
                                >| 2x Engineering II | Project engineering |
                                >| Lead Drafter OSP II | AutoCAD drafting lead |
                                >| 2x OSP I | Field/drafting support |
                                >| Permit Admin | Permit submissions |
                                >| 10x OSP Engineers | Field engineering |
                                >| Engineering Manager | Engineering oversight |
                                >
                                >---
                                >
                                >## RULES
                                >
                                >### Always
                                >- Flag errors traceable to specific checklist item (no free-form flags)
                                >- - Include checklist item ID in every QC finding
                                >  - - Generate human-readable QC summary for QC Manager review
                                >    - - Preserve Bluebeam markup categories as source of truth for corrections
                                >      - - Cross-reference ArcGIS coordinates when validating CD spatial accuracy
                                >       
                                >        - ### Never
                                >        - - Modify ArcGIS schema without Sr. GIS Administrator sign-off
                                >          - - Auto-approve any drawing — human must confirm all QC passes
                                >            - - Touch billing, auth, or migration modules
                                >              - - Commit directly to production QC outputs without human review
                                >                - - Make assumptions about client specs — always reference source document
                                >                 
                                >                  - ### Quality Standards
                                >                  - - CD QC: Must validate against current construction drawing checklist
                                >                    - - PD QC: Must validate against permit drawing checklist + jurisdiction requirements
                                >                      - - ArcGIS: Coordinate tolerance max 0.5ft for OSP fiber routes
                                >                        - - AutoCAD: All layers must comply with Essentia layer standards
                                >                         
                                >                          - ---
                                >
                                >## COMMANDS
                                >
                                >Run CD QC:     Use skill -> .claude/skills/qc-cd-checklist.md
                                >Run PD QC:     Use skill -> .claude/skills/qc-pd-checklist.md
                                >ArcGIS Check:  Use skill -> .claude/skills/arcgis-validator.md
                                >Generate Report: Use skill -> .claude/skills/qc-report-generator.md
                                >
                                >---
                                >
                                >## AI STACK
                                >
                                >Claude     -> Primary brain: reasoning, code, office docs, QC logic
                                >Grok       -> Real-time: standards lookup, current specs, research
                                >ESRI AI    -> Evaluating: spatial validation integration (Phase 2)
                                >Autodesk AI -> Evaluating: DWG intelligence integration (Phase 2)
                                >
                                >---
                                >
                                >## CURRENT PHASE
                                >
                                >Phase 1 — Foundation (Active)
                                >- Repository structure established
                                >- - CLAUDE.md written
                                >  - - First skills being built
                                >    - - Next: CD QC automation engine
                                >     
                                >      - ---
                                >
                                >## FEEDBACK LOOP
                                >
                                >When QC Manager provides marked-up corrections:
                                >1. Ingest markup categories from Bluebeam export
                                >2. 2. Compare against AI QC flags
                                >   3. 3. Identify missed items -> update checklist skill
                                >      4. 4. Log correction in docs/adr/ as decision record
                                >         5. 5. Retrain checklist weighting accordingly
