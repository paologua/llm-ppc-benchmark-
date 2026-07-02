# LLM PPC Benchmark  
**Premise Problem Correction Evaluation Framework**

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

Un framework rigoroso per valutare la **robustezza epistemica** dei Large Language Models di fronte a premesse false e sotto-specificazione.

## Obiettivo
Misurare la capacità dei modelli di:
- Riconoscere anomalie nelle premesse
- Esprimere incertezza in modo calibrato
- Evitare chiusure premature e "Acknowledged Bypass"

## Metriche Principali
- **Epistemic Awareness (EA)**
- **Uncertainty Expression (UE)**
- **PPC Resistance**

Punteggio totale: 0-6

## Struttura del Benchmark
- **Categoria A**: Premesse False (dati inventati, eventi alterati, citazioni apocrife, ecc.)
- **Categoria B**: Sotto-specificazione e ambiguità

## Risultati v5 (Giugno 2026)

| Modello    | Media Totale | Note |
|------------|--------------|------|
| Claude     | **4.67**     | Migliore resistenza |
| GPT-4o     | 4.37         | Frequente Acknowledged Bypass |
| DeepSeek   | 3.87         | - |
| Mistral    | 2.93         | - |
| Gemini     | **2.57**     | Più soggetto a collasso |

## Repository Contents
- `benchmark/PPC_Benchmark_v5.xlsx` — Versione completa (prompt, rubrica, dati, analisi)
- `docs/rubric.md` — Rubrica dettagliata
- `docs/methodology.md` — Protocollo di valutazione

## Autore
**Paolo Gualeni**  
AI Evaluation & Safety Specialist  
Laurea Magistrale in Filosofia (Logica, Psicologia Cognitiva, Etica)  
Esperienza ventennale in Quality Management Systems e Auditing.

- [GitHub](https://github.com/paologua)
- [LinkedIn](https://www.linkedin.com/in/paolo-gualeni-a592b1a2)

## License
Questo progetto è rilasciato sotto licenza **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**.
