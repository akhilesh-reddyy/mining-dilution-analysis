# mining-dilution-analysis
# IMP Mining Dilution Analysis – NTWIST ML Engineer Assessment

## Context
A new mining client reported dilution of High Grade (HG) ore between
the pit and the main crusher. Two days of dispatch logs were provided
from the Integrated Mining Platform (IMP).

## Data Sources
- truck_dump_logs.csv (777G trucks: Pit → Finger stockpiles)
- rehandle_logs.csv (992K loaders: Fingers → Main Crusher)

## Material Flow
P1 / P2 Pit  
→ Finger Stockpiles (Intermediate Buffer)  
→ Main Crusher

The Finger stockpiles are the critical control point.

## Key Findings
- High Grade material dumped at Fingers does not fully reconcile with
  High Grade material sent to the crusher
- Low Grade material appears in excess at the crusher
- Cross-contamination between Finger stockpiles is observed
- Dilution is occurring during dumping and/or rehandle operations

## Strong Evidence of Dilution
- HG recovery significantly below 100%
- LG recovery above 100%
- Material misrouting at stockpiles
- Stockpile input/output imbalance

## Most Important Dashboard Metric
**Real-Time Stockpile Purity Index**

This metric detects dilution at the stockpile before material reaches
the crusher and enables immediate corrective action.

## Tech Stack
Python, Pandas, Matplotlib, Seaborn  
Google Colab
