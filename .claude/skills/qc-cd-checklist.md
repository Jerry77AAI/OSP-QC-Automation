# SKILL: QC Construction Drawing (CD) Checklist
## Expert Mode — OSP QC Automation Consortium

---

## ACTIVATION

When this skill is active, Claude enters CD QC Expert Mode.
Review every Construction Drawing against ALL checklist items below.
Flag any non-compliance with item ID, description, and severity.

---

## OUTPUT FORMAT

For each drawing reviewed, produce:

### QC REPORT — [Drawing Number] — [Date]
- PASS / FAIL / CONDITIONAL
- - Total Items Checked: XX
  - - Flags: XX Critical | XX Major | XX Minor
   
    - | Item ID | Category | Finding | Severity | Action Required |
    - |---------|----------|---------|----------|-----------------|
    - | CD-001 | Title Block | Missing PE stamp | CRITICAL | Reject — return to engineer |
   
    - ---

    ## CHECKLIST — CONSTRUCTION DRAWINGS

    ### TITLE BLOCK (TB)
    - [ ] TB-001 | Drawing number matches project log
    - [ ] - [ ] TB-002 | Revision number current and matches markup
    - [ ] - [ ] TB-003 | PE stamp present and current (not expired)
    - [ ] - [ ] TB-004 | Client name correct
    - [ ] - [ ] TB-005 | Project name and address correct
    - [ ] - [ ] TB-006 | Date of issue correct
    - [ ] - [ ] TB-007 | Scale indicated and correct
    - [ ] - [ ] TB-008 | Sheet number and total sheets correct
   
    - [ ] ### GENERAL NOTES (GN)
    - [ ] - [ ] GN-001 | General notes present and complete
    - [ ] - [ ] GN-002 | Notes reference correct spec version
    - [ ] - [ ] GN-003 | Material specs match BOM
    - [ ] - [ ] GN-004 | Construction notes match field conditions
   
    - [ ] ### FIBER ROUTE (FR)
    - [ ] - [ ] FR-001 | Route matches approved alignment
    - [ ] - [ ] FR-002 | Fiber type and count labeled correctly
    - [ ] - [ ] FR-003 | Conduit size and type labeled
    - [ ] - [ ] FR-004 | Bore/directional drill locations marked
    - [ ] - [ ] FR-005 | Splice locations shown with correct icon
    - [ ] - [ ] FR-006 | Slack loop locations shown
    - [ ] - [ ] FR-007 | Pulling tension notes present at bends
   
    - [ ] ### POLE ATTACHMENT (PA)
    - [ ] - [ ] PA-001 | Pole numbers match utility records
    - [ ] - [ ] PA-002 | Make-ready requirements noted
    - [ ] - [ ] PA-003 | Attachment height shown
    - [ ] - [ ] PA-004 | Down guy / anchor locations shown if required
    - [ ] - [ ] PA-005 | Clearance distances noted
   
    - [ ] ### UNDERGROUND PLACEMENT (UG)
    - [ ] - [ ] UG-001 | Duct bank depth shown (min 24" telecom)
    - [ ] - [ ] UG-002 | Warning tape noted
    - [ ] - [ ] UG-003 | Conduit fill ratio acceptable (<40%)
    - [ ] - [ ] UG-004 | Bore pit locations shown
    - [ ] - [ ] UG-005 | Road crossing permits referenced
   
    - [ ] ### ARCGIS / SPATIAL (GIS)
    - [ ] - [ ] GIS-001 | GPS coordinates on all splice points
    - [ ] - [ ] GIS-002 | Coordinate system noted (NAD83 preferred)
    - [ ] - [ ] GIS-003 | Route length matches ArcGIS measurement (+/- 2%)
    - [ ] - [ ] GIS-004 | Existing utilities shown from JULIE/811 data
    - [ ] - [ ] GIS-005 | Conflict zones flagged
   
    - [ ] ### AS-BUILT COMPLIANCE (AB)
    - [ ] - [ ] AB-001 | Drawing matches field-verified route
    - [ ] - [ ] AB-002 | No unauthorized deviations from permit
    - [ ] - [ ] AB-003 | Change order reflected if route modified
   
    - [ ] ---
   
    - [ ] ## SEVERITY DEFINITIONS
   
    - [ ] | Level | Definition | Action |
    - [ ] |-------|-----------|--------|
    - [ ] | CRITICAL | Regulatory / safety #v iSoKlIaLtLi:o nQ C|  CRoenjsetcrtu citmimoend iDartaewliyn g|
    - [ ] (|C DM)A JCOhRe c|k lWiisltl
    - [ ]  #c#a uEsxep efrite lMdo deer r— oOrS Po rQ Cr eAwuotrokm a|t iRoenj eCcotn s— ofritxi ubme
    - [ ]  f
    - [ ]  o-r-e-
    - [ ]  i
    - [ ]  s#s#u eA C|T
    - [ ]  I|V AMTIINOONR
   
    - [ ]   |W hDeonc utmheinst astkiiolnl  giasp  a|c tFilvaeg,  —C lfaiuxd ea te nnteexrts  rCeDv iQsCi oEnx p|e
    - [ ]   r|t  NMOoTdEe .|
    - [ ]    RBeevsite wp reavcetriyc eC osnusgtgreuscttiioonn  |D rLaowgi nfgo ra geanignisnte eArL La wcahreecnkelsiss t|
    - [ ]    i
    - [ ]    t-e-m-s
   
    - [ ]     b#e#l oRwU.L
    - [ ] EFSl aFgO Ra nTyH InSo nS-KcIoLmLp
    - [ ] l
    - [ ] i-a nNceev ewri tmha rikt ePmA SISD ,i fd easncyr iCpRtIiToInC,A La nodr  sMeAvJeOrRi tiyt.e
    - [ ] m
    - [ ] s- -a-r
    - [ ] e
    - [ ]  #f#l aOgUgTePdU
    - [ ]  T-  FAOlRwMaAyTs
   
    - [ ]   iFnocrl uedaec hc hdercakwliinsgt  rietveime wIeDd ,i np reovdeurcye :f
    - [ ]   i
    - [ ]   n#d#i#n gQ
    - [ ]   C-  RIEfP OdRrTa w—i n[gD rcaawninnogt  Nbuem breerv]i e— w[eDda t(ei]l
    - [ ]   l-e gPiAbSlSe ,/  mFiAsIsLi n/g  CsOhNeDeItTsI)O,N AfLl
    - [ ]   a-g  Taost aIlN CIOtMePmLsE TCEh
    - [ ]   e-c kCerdo:s sX-Xr
    - [ ]   e-f eFrleangcse:  AXrXc GCIrSi tdiactaal  f|o rX Xa lMla jGoIrS -|0 0X1X  tMhirnoourg
    - [ ]   h
    - [ ]    |G IISt-e0m0 5I Di t|e mCsa
    - [ ]    t-e gRooruyt e|  fFiinnddiinnggs  |t oS eQvCe rMiatnya g|e rA cbteifoonr eR erqeutiurrendi n|g
    - [ ]     |t-o- -e-n-g-i-n-e-e|r----------|---------|----------|-----------------|
    - [ ] | CD-001 | Title Block | Missing PE stamp | CRITICAL | Reject — return to engineer |
   
    - [ ] ---
   
    - [ ] ## CHECKLIST — CONSTRUCTION DRAWINGS
   
    - [ ] ### TITLE BLOCK (TB)
    - [ ] - [ ] TB-001 | Drawing number matches project log
    - [ ] - [ ] TB-002 | Revision number current and matches markup
    - [ ] - [ ] TB-003 | PE stamp present and current (not expired)
    - [ ] - [ ] TB-004 | Client name correct
    - [ ] - [ ] TB-005 | Project name and address correct
    - [ ] - [ ] TB-006 | Date of issue correct
    - [ ] - [ ] TB-007 | Scale indicated and correct
    - [ ] - [ ] TB-008 | Sheet number and total sheets correct
   
    - [ ] ### GENERAL NOTES (GN)
    - [ ] - [ ] GN-001 | General notes present and complete
    - [ ] - [ ] GN-002 | Notes reference correct spec version
    - [ ] - [ ] GN-003 | Material specs match BOM
    - [ ] - [ ] GN-004 | Construction notes match field conditions
   
    - [ ] ### FIBER ROUTE (FR)
    - [ ] - [ ] FR-001 | Route matches approved alignment
    - [ ] - [ ] FR-002 | Fiber type and count labeled correctly
    - [ ] - [ ] FR-003 | Conduit size and type labeled
    - [ ] - [ ] FR-004 | Bore/directional drill locations marked
    - [ ] - [ ] FR-005 | Splice locations shown with correct icon
    - [ ] - [ ] FR-006 | Slack loop locations shown
    - [ ] - [ ] FR-007 | Pulling tension notes present at bends
   
    - [ ] ### POLE ATTACHMENT (PA)
    - [ ] - [ ] PA-001 | Pole numbers match utility records
    - [ ] - [ ] PA-002 | Make-ready requirements noted
    - [ ] - [ ] PA-003 | Attachment height shown
    - [ ] - [ ] PA-004 | Down guy / anchor locations shown if required
    - [ ] - [ ] PA-005 | Clearance distances noted
   
    - [ ] ### UNDERGROUND PLACEMENT (UG)
    - [ ] - [ ] UG-001 | Duct bank depth shown (min 24" telecom)
    - [ ] - [ ] UG-002 | Warning tape noted
    - [ ] - [ ] UG-003 | Conduit fill ratio acceptable (<40%)
    - [ ] - [ ] UG-004 | Bore pit locations shown
    - [ ] - [ ] UG-005 | Road crossing permits referenced
   
    - [ ] ### ARCGIS / SPATIAL (GIS)
    - [ ] - [ ] GIS-001 | GPS coordinates on all splice points
    - [ ] - [ ] GIS-002 | Coordinate system noted (NAD83 preferred)
    - [ ] - [ ] GIS-003 | Route length matches ArcGIS measurement (+/- 2%)
    - [ ] - [ ] GIS-004 | Existing utilities shown from JULIE/811 data
    - [ ] - [ ] GIS-005 | Conflict zones flagged
   
    - [ ] ### AS-BUILT COMPLIANCE (AB)
    - [ ] - [ ] AB-001 | Drawing matches field-verified route
    - [ ] - [ ] AB-002 | No unauthorized deviations from permit
    - [ ] - [ ] AB-003 | Change order reflected if route modified
   
    - [ ] ---
   
    - [ ] ## SEVERITY DEFINITIONS
   
    - [ ] | Level | Definition | Action |
    - [ ] |-------|-----------|--------|
    - [ ] | CRITICAL | Regulatory / safety violation | Reject immediately |
    - [ ] | MAJOR | Will cause field error or rework | Reject — fix before issue |
    - [ ] | MINOR | Documentation gap | Flag — fix at next revision |
    - [ ] | NOTE | Best practice suggestion | Log for engineer awareness |
   
    - [ ] ---
   
    - [ ] ## RULES FOR THIS SKILL
   
    - [ ] - Never mark PASS if any CRITICAL or MAJOR items are flagged
    - [ ] - Always include checklist item ID in every finding
    - [ ] - If drawing cannot be reviewed (illegible, missing sheets), flag as INCOMPLETE
    - [ ] - Cross-reference ArcGIS data for all GIS-001 through GIS-005 items
    - [ ] - Route findings to QC Manager before returning to engineer
