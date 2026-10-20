# Formal Text AI Detection Dataset

A repository dedicated to collecting a dataset for testing synthetic (AI-generated) text detection pipelines.

## Overview
The present task is gathering high-quality, formal text datasets—specifically **research paper abstracts**, to evaluate how well detection pipelines perform on complex, academic writing styles.

## To Be Added Later
* APIs Used for Collection
* Models Being Used for detection

## Navigation
| Folder | Description |
|---|---|
| abstract retrieval | contains the actual abstracts collected through retrieval pipelines, for each conference:<br>1. total abstract datasets - complete bulk data retrieved<br>2. retrieval reports - metadata of the retrieval (count of missing, found etc.)<br>3. auxiliary data - checkpoints (loss prevention) and api catalogues<br>4. usable abstracts - the actual usable abstracts with length > 50 tokens used further in detection pipelines |
| post gpt papers / pre gpt papers | the complete metadata retrieved about the paper through its DBLP key, to help abstract retrieval |
| results | the actual results obtained against each abstract after passing the usable abstracts through detection pipelines across all 4 detectors |
| analysis | comprehensive combination of all results in visual and tabular formats<br>most important results:<br>tabular \| visual<br>01-all_conferences_grouped_bar_comparison \| 01-master_all_conferences_comparison<br>02-overall_weighted_model_comparison \| 02-overall_model_comparison<br>rest ---> individual tables and bar graphs for all six conferences |

<!-- PAPER-COUNT-START -->
## Current count of **Abstracts**

| Conference | Pre-GPT Abstracts | Post-GPT Abstracts |
|---|---:|---:|
| AAAI | 4805 | 6537 |
| CSCW | 704 | 1364 |
| ICLR | 650 | 3627 |
| ICML | 1512 | 5237 |
| ICWSM | 883 | 344 |
| NeurIPS | 2183 | 9756 |

Pre-GPT papers include publications up to and including 2018.  
Post-GPT papers include publications from 2023 through 2025.

<!-- PAPER-COUNT-END -->
