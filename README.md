# Protocol for the preparation of genomic DNA via NaOH lysis using the Opentrons OT-2 Pipetting Robot
A protocol for preparing genomic DNA from a 300 well plate for PCR genotyping, followed by PCR prep of tubes. Developed and tested using <5dpf larval zebrafish (*Danio rerio*) in the [Randlett Lab](https://randlettlab.com/) at the [MeLiS Institute](https://inmg.fr/melis/fr/index.php) (Mécanismes en sciences intégratives du vivant) at Université Claude Bernard Lyon 1.
The code is written in Python using the [Opentrons API](https://docs.opentrons.com/v2/) and run in the code cells of Jupyter.

<img width="572" alt="Screen Shot 2024-01-26 at 8 59 39 AM" src="https://github.com/andrewhsiao11/opentrons_pipetting_robot/assets/90870850/3e243255-29f1-4754-98fc-580bcbddec25"> <img width="339" alt="Screen Shot 2024-01-26 at 12 59 32 PM" src="https://github.com/andrewhsiao11/opentrons_pipetting_robot/assets/90870850/d3cd8819-baf2-46f7-834a-93ad06875c6e">

## TLDR
- NaOH directly to wells
- Heat plate in oven for 15 minutes 
- Tris-HCL directly to wells
- DNA transferred to gDNA plates
- Master Mix dispensed to PCR tubes

-------
## Setup
This setup uses Fisher 96 200ul tip racks, 96 well gDNA plates, in-lab made 300 well plate to hold individual zebrafish larvae, 50ml Falcon tubes, and 2ml Eppendorf tubes. 
<img width="782" alt="Screen Shot 2024-01-26 at 1 18 18 PM" src="https://github.com/andrewhsiao11/opentrons_pipetting_robot/assets/90870850/cce11928-d850-47d0-bce4-77a02bbdf40c">

### Details on how the combirack is defined as a labware (A1...A5, B1...B12)

<img width="529" alt="Screen Shot 2024-01-26 at 1 38 55 PM" src="https://github.com/andrewhsiao11/opentrons_pipetting_robot/assets/90870850/20cd6d18-44e0-444e-a475-8d72f592fee7">
