## Curated Paper List for LLMs as Agent and LLMs for Tool Use.

This repo contains a curated list of papers relating to recent literature of LLMs as Agent and LLMs for Tool Use. We welcome the community to contribute and add papers to the list that you find enjoyable to read.


* **[2023.02.09] Toolformer: Language Models Can Teach Themselves to Use Tools** [[arxiv]](https://arxiv.org/abs/2302.04761) [[code]]()

  _Authors: Timo Schick, Jane Dwivedi-Yu, Roberto Dessì†, Roberta Raileanu, Maria Lomeli, Luke Zettlemoyer, Nicola Cancedda, Thomas Scialo._

  <details>
  <summary>[Takeaways]:</summary>
    Teach LLMs to use tools by generating text and API calls (represented by text) in an interleaved manner. The training corpus is constructed on CCNet with some predefined heuristics. Experiments on various benchmarks, e.g. LAMA, Math, Question Answering, demonstrate zero-shot strong performance over much larger LLMs (OPT and GPT-3) without providing any in-context examples. The remaining challenges in Toolformer is its inability (i) to use multiple tools when addressing natural language task, (ii) to discard the output from APIs by itself when the output is not helpful.
  </details>

* **[2023.08.22] Language agents: a critical evolutionary step of artificial intelligence** [[slides]](https://lfs.aminer.cn/misc/language_agents_YuSu.pdf)

  _Authors: Yu Su_

  <details>
  <summary>[Takeaways]:</summary>
    Discuss the definition of (1) LLMs as agents, (2) tool augmentation, (3) reasoning and planning, (4) grounding.
  </details>
