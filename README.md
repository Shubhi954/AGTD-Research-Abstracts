# Formal Text AI Detection Dataset

A repository dedicated to collecting a dataset for testing synthetic (AI-generated) text detection pipelines.

## Overview
The present task is gathering high-quality, formal text datasets—specifically **research paper abstracts**, to evaluate how well detection pipelines perform on complex, academic writing styles.

## To Be Added Later
* APIs Used for Collection
* Models Being Used for detection

## Navigation

<table>
  <thead>
    <tr>
      <th>Folder</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="./abstract%20retrieval/">abstract retrieval</a></td>
      <td>
        contains the actual abstracts collected through retrieval pipelines, for each conference:
        <ol>
          <li>total abstract datasets - complete bulk data retrieved</li>
          <li>retrieval reports - metadata of the retrieval (count of missing, found etc.)</li>
          <li>auxiliary data - checkpoints (loss prevention) and api catalogues</li>
          <li>usable abstracts - the actual usable abstracts with length &gt; 50 tokens used further in detection pipelines</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td>
        <a href="./post%20gpt%20papers/">post gpt papers</a> /
        <a href="./pre%20gpt%20papers/">pre gpt papers</a>
      </td>
      <td>the complete metadata retrieved about the paper through its DBLP key, to help abstract retrieval</td>
    </tr>
    <tr>
      <td><a href="./results/">results</a></td>
      <td>the actual results obtained against each abstract after passing the usable abstracts through detection pipelines across all 4 detectors</td>
    </tr>
    <tr>
      <td><a href="./analysis/">analysis</a></td>
      <td>
        comprehensive combination of all results in visual and tabular formats
        <p>most important results:</p>
        <table>
          <thead>
            <tr>
              <th>tabular</th>
              <th>visual</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td><a href="./analysis/01-all_conferences_grouped_bar_comparison">01-all_conferences_grouped_bar_comparison</a></td>
              <td><a href="./analysis/01-master_all_conferences_comparison">01-master_all_conferences_comparison</a></td>
            </tr>
            <tr>
              <td><a href="./analysis/02-overall_weighted_model_comparison">02-overall_weighted_model_comparison</a></td>
              <td><a href="./analysis/02-overall_model_comparison">02-overall_model_comparison</a></td>
            </tr>
          </tbody>
        </table>
        <p>rest ---&gt; individual tables and bar graphs for all six conferences</p>
      </td>
    </tr>
  </tbody>
</table>


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
