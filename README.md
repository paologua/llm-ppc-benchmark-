# PPC Benchmark  
**Premise Problem Correction Evaluation Framework**

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
![Version](https://img.shields.io/badge/version-v5.0-blue)

**Un framework rigoroso per valutare la robustezza epistemica dei Large Language Models.**

## Introduzione

Il **PPC Benchmark** misura quanto i modelli siano capaci di resistere a input problematici, distinguendo tra:

- **Premesse false** (dati inventati, eventi storici alterati, citazioni apocrife, causalità invertite…)
- **Sotto-specificazione** (ambiguità, dati insufficienti, generalizzazioni indebite…)

L’obiettivo non è solo verificare la correttezza fattuale, ma valutare la **costanza epistemica**: la capacità del modello di riconoscere limiti, esprimere incertezza calibrata e evitare chiusure premature.

## Metriche Principali (0-2 ciascuna, totale 0-6)

1. **Epistemic Awareness (EA)**  
   Riconoscimento esplicito di anomalie nella premessa.

2. **Uncertainty Expression (UE)**  
   Espressione di incertezza genuina e strutturata (non hedging retorico).

3. **PPC Resistance**  
   Resistenza alla chiusura cognitiva e all’*Acknowledged Bypass* (riconosce l’errore ma procede comunque a rispondere come se fosse valido).

## Contenuti del Repository

- `benchmark/PPC_Benchmark_v5.xlsx` — Versione completa (prompts, rubrica, dati grezzi, analisi)
- `docs/rubric.md` — Rubrica dettagliata con esempi anchor
- `docs/methodology.md` — Protocollo di somministrazione e valutazione
- `examples/` — Casi annotati
- `results/` — Analisi aggregate e grafici

## Risultati Principali (v5 — Giugno 2026)

| Modello    | Media Totale | Categoria A (False Premises) | Categoria B (Underspecification) | Note principali |
|------------|--------------|------------------------------|----------------------------------|-----------------|
| Claude     | **4.67**     | Alto                         | Alto                             | Migliore resistenza complessiva |
| GPT-4o     | 4.37         | Medio-Alto                   | Medio                            | Frequente Acknowledged Bypass |
| DeepSeek   | 3.87         | Medio                        | Medio                            | - |
| Mistral    | 2.93         | Basso                        | Basso                            | - |
| Gemini     | **2.57**     | Basso                        | Basso                            | Alto tasso di collasso |

**Failure modes più frequenti**: Acknowledged Bypass, Narrative Projection, Claim Acceptance Without Verification.

## Come Usarlo

1. Aprire una sessione pulita (New Chat) per ogni prompt
2. Applicare la rubrica dettagliata
3. Registrare score e output rappresentativi
4. Confrontare con i risultati di riferimento

## Autore

**Paolo Gualeni**  
AI Reasoning & Safety Evaluator | Data Quality Specialist  
Formazione: Laurea Magistrale in Filosofia (Logica Formale, Psicologia Cognitiva, Etica)  
Background professionale: Quality Management Systems (ISO 9000), Auditing, Operations.

- GitHub: [paologua](https://github.com/paologua)
- LinkedIn: [paolo-gualeni](https://www.linkedin.com/in/paolo-gualeni-a592b1a2)
- Email: nex.dpg@gmail.com

## Citazione

```bibtex
@misc{gualeni2026ppc,
  author       = {Gualeni, Paolo},
  title        = {PPC Benchmark: Premise Problem Correction},
  year         = {2026},
  publisher    = {GitHub},
  howpublished = {\url{https://github.com/paologua/PPC-Benchmark}},
}
