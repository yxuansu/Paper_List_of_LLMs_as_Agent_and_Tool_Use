## Curated Paper List for LLMs as Agent and LLMs for Tool Use.

This repo contains a curated list of papers relating to recent literature of LLMs as Agent and LLMs for Tool Use. We welcome the community to contribute and add papers to the list that you find enjoyable to read.


* **[2023.02.09] Toolformer: Language Models Can Teach Themselves to Use Tools** [[arxiv]](https://arxiv.org/abs/2302.04761) 

  _[Authors]: Timo Schick, Jane Dwivedi-Yu, Roberto Dessì†, Roberta Raileanu, Maria Lomeli, Luke Zettlemoyer, Nicola Cancedda, Thomas Scialo._

  <details open>
  <summary>[Takeaways]: (click to close)</summary>
    Teach LLMs to use tools by generating text and API calls (represented by text) in an interleaved manner. The training corpus is constructed on CCNet with some predefined heuristics. Experiments on various benchmarks, e.g. LAMA, Math, Question Answering, demonstrate zero-shot strong performance over much larger LLMs (OPT and GPT-3) without providing any in-context examples. The remaining challenges in Toolformer is its inability (i) to use multiple tools when addressing natural language task, (ii) to discard the output from APIs by itself when the output is not helpful.
  </details>

* **[2023.08.07] AgentBench: Evaluating LLMs as Agents** [[arxiv]](https://arxiv.org/abs/2308.03688) [[code]](https://github.com/THUDM/AgentBench)

  _[Authors]: Xiao Liu, Hao Yu, Hanchen Zhang, Yifan Xu, Xuanyu Lei, Hanyu Lai, Yu Gu, Hangliang Ding, Kaiwen Men, Kejuan Yang, Shudan Zhang, Xiang Deng, Aohan Zeng, Zhengxiao Du, Chenhui Zhang, Sheng Shen, Tianjun Zhang,
Yu Su, Huan Sun, Minlie Huang, Yuxiao Dong, Jie Tang_

  <details open>
  <summary>[Takeaways]: (click to close)</summary>
    AgentBench consists of 8 distinct environment to assess the capabilities of LLMs as agenst, including
    
    * (1) Operating System (OS)
    * (2) Database (DB)
    * (3) Knowledge Graph (KG)
    * (4) Digital Card Game (DCG)
    * (5) Lateral Thinking Puzzles (LTP)
    * (6) House-holding (Alfworld)
    * (7) Web Shopping (WebShop)
    * (8) Web Browsing (Mind2Web)
  </details>

  

* **[2023.08.22] Language agents: a critical evolutionary step of artificial intelligence** [[slides]](https://lfs.aminer.cn/misc/language_agents_YuSu.pdf)

  _[Author]: Yu Su_

  <details open>
  <summary>[Takeaways]: (click to close)</summary>
    Discuss the definition of (1) LLMs as agents, (2) tool augmentation, (3) reasoning and planning, (4) grounding.
  </details>
