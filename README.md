## Curated Paper List for LLMs as Agent and LLMs for Tool Use.

This repo contains a curated list of papers relating to recent literature of LLMs as Agent and LLMs for Tool Use. We welcome the community to contribute and add papers to the list that you find enjoyable to read.


* **Toolformer: Language Models Can Teach Themselves to Use Tools** 

  _Timo Schick, Jane Dwivedi-Yu, Roberto Dessì†, Roberta Raileanu, Maria Lomeli, Luke Zettlemoyer, Nicola Cancedda, Thomas Scialom_
  
  [[Arxiv]](https://arxiv.org/abs/2302.04761) [Code]()

  <details>
  <summary>Takeaways:</summary>
    Teach LLMs to use tools by generating text and API calls (represented by text) in an interleaved manner. The training corpus is constructed on CCNet with some predefined heuristics. Experiments on various benchmarks, e.g. LAMA, Math, Question Answering, demonstrate zero-shot strong performance over much larger LLMs (OPT and GPT-3) without providing any in-context examples. The remaining challenges in Toolformer is its inability (i) to use multiple tools when addressing natural language task, (ii) to discard the output from APIs by itself when the output is not helpful.
  </details>
