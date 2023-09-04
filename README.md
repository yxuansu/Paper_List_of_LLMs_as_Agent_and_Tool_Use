## Curated Paper List for LLMs as Agent and LLMs for Tool Use.

This repo contains a curated list of papers relating to recent literature of LLMs as Agent and LLMs for Tool Use. We welcome the community to contribute and add papers to the list that you find enjoyable to read.


* **[2023.02.09] Toolformer: Language Models Can Teach Themselves to Use Tools** [[arxiv]](https://arxiv.org/abs/2302.04761) 

  _[Authors]: Timo Schick, Jane Dwivedi-Yu, Roberto Dessì†, Roberta Raileanu, Maria Lomeli, Luke Zettlemoyer, Nicola Cancedda, Thomas Scialo._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
    Teach LLMs to use tools by generating text and API calls (represented by text) in an interleaved manner. The training corpus is constructed on CCNet with some predefined heuristics. Experiments on various benchmarks, e.g. LAMA, Math, Question Answering, demonstrate zero-shot strong performance over much larger LLMs (OPT and GPT-3) without providing any in-context examples. The remaining challenges in Toolformer is its inability (i) to use multiple tools when addressing natural language task, (ii) to discard the output from APIs by itself when the output is not helpful.


    Toolformer considers a limited number of tools, including (1) Question Answering; (2) Calculator; (3) Wikipedia Search; (4) Machine Translation System; and (5) Calendar. And it focuses on single tool-usage scenerios.
  </details>

* **[2023.05.24] Chameleon: Plug-and-Play Compositional Reasoning with Large Language Models** [[arxiv]](https://arxiv.org/abs/2304.09842) [[code]](https://github.com/lupantech/chameleon-llm)

  _[Authors]: Pan Lu, Baolin Peng, Hao Cheng, Michel Galley, Kai-Wei Chang, Ying Nian Wu, Song-Chun Zhu, Jianfeng Gao._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
    Propose a plug-and-play framework to address multi-modal reasoning task. The core component is a LLM-powered planner which is surrounded by a few dedicated tool modules. Some of the tools are implemented with LLMs by prompting with few-shot demonstrations. Chameleon demonstrates promising results on two challenging benchmarks.
  </details>


* **[2023.05.24] Gorilla: Large Language Model Connected with Massive APIs** [[arxiv]](https://arxiv.org/abs/2305.15334) [[code]](https://gorilla.cs.berkeley.edu/)

  _[Authors]: Shishir G. Patil, Tianjun Zhang, Xin Wang, Joseph E. Gonzalez._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
    Gorilla focuses on the single-turn and single tool-usage (i.e. one API call) scenarios. Gorilla proposes APIBench which collects tools from Huggingface, Torch, and TensorFlow. The instruction-answer pairs are synthetically created by prompting GPT-4. Gorilla considers two different setting: (1) zero-shot and (2) retriever, in which a retriever (e.g. BM25, GPT-Index, or Oracle) is a involved. The experimental results demonstrate that when the quality of the retriever is low, the performance of the model could be even decreased.

    In one word, Gorilla is a nice work pioneering the field of API usage with LLMs.
  </details>


* **[2023.05.25] On the Tool Manipulation Capability of Open-source Large Language Models** [[arxiv]](https://arxiv.org/abs/2305.16504) [[code]](https://github.com/sambanova/toolbench)

  _[Authors]: Qiantong Xu, Fenglu Hong, Bo Li, Changran Hu, Zhengyu Chen, Jian Zhang._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
    This work identifies three main challenges posed to open-source LLMs for tool use, namely, (1) difficulty in API selection; (2) confusion in populating arguments; and (3) non-executable generation. It leverages LLMs for tool use by following a standard paradigm: instruction -> action generation -> observation -> final output. This work proposes a ToolBench which gathers popular APIs from sites like REST APIs (https://openweathermap.org/api) and (https://thecatapi.com/). The experimental results show promising improvements given the authors' proposed approaches. 
  </details>



* **[2023.05.30] GPT4Tools: Teaching Large Language Model to Use Tools via Self-instruction** [[arxiv]](https://arxiv.org/abs/2305.18752) [[code]](https://github.com/StevenGrove/GPT4Tools)

  _[Authors]:Rui Yang, Lin Song, Yanwei Li, Sijie Zhao, Yixiao Ge, Xiu Li, Ying Shan._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
    This work investigates LLMs tool use for multimodal scenarios. The definitions of multimodal tools are similar to Visual ChatGPT. The evaluation benchmark is synthetically generated with ChatGPT.
  </details>
  

* **[2023.07.31] ToolLLM: Facilitating Large Language Models To Master 16000+ Real-World APIs** [[arxiv]](https://arxiv.org/abs/2307.16789) [[code]](https://github.com/OpenBMB/ToolBench)

  _[Authors]:Yujia Qin, Shihao Liang, Yining Ye, Kunlun Zhu, Lan Yan, Yaxi Lu, Yankai Lin , Xin Cong, Xiangru Tang, Bill Qian, Sihan Zhao, Runchu Tian, Ruobing Xie, Jie Zhou, Mark Gerstein, Dahai Li, Zhiyuan Liu, Maosong Sun._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
    Gather up 3451 tools (e.g. social media, e-commerce, and weather) consisting of 16464 APIs from RapidAPI (https://rapidapi.com/hub). The benchmark is synthetically generated by prompting ChatGPT. The instructions cover both single- and multi-tool usage for practical usage. The evaluation consists of two aspetcs: (1) pass rate; (2) win rate. A DFS-based method is proposed to improve the reasoning capabilities of ToolLLM.

    Comparing to Toolformer, ToolLLM considers more fine-grained categorizations of tools. For instance, each class of tool (e.g. Movie) consists of multiple subtools, such as (1) Star Wars Characters; (2) Streaming Availability; and etc. This fine-grained categorization offers the LLMs with more fleixibility and the capability to operate in a more precise way. Inevitably, it also demands the LLMs to identify nuanced distinctions between similar tools in order to complete the task.
  </details>


* **[2023.08.01] Tool Documentation Enables Zero-Shot Tool-Usage with Large Language Models** [[arxiv]](https://arxiv.org/abs/2308.00675)

  _[Authors]: Cheng-Yu Hsieh, Si-An Chen, Chun-Liang Li, Yasuhisa Fujii, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, Tomas Pfister._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
    This work presents a straightforward but important conclusion. When teaching LLMs to use tools, documentations are often more efficient and scalable comparing to the conventional ways of providing few-shot demonstrations (e.g. in-context examples of how to use (several) tool(s) to address a specific task). 

    I personally like this paper a lot.
  </details>
  
  

* **[2023.08.07] AgentBench: Evaluating LLMs as Agents** [[arxiv]](https://arxiv.org/abs/2308.03688) [[code]](https://github.com/THUDM/AgentBench)

  _[Authors]: Xiao Liu, Hao Yu, Hanchen Zhang, Yifan Xu, Xuanyu Lei, Hanyu Lai, Yu Gu, Hangliang Ding, Kaiwen Men, Kejuan Yang, Shudan Zhang, Xiang Deng, Aohan Zeng, Zhengxiao Du, Chenhui Zhang, Sheng Shen, Tianjun Zhang,
Yu Su, Huan Sun, Minlie Huang, Yuxiao Dong, Jie Tang._

  <details open>
  <summary><b>[Remarks]</b>: (click to close)</summary>
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
  <summary><b>[Remarks]</b>: (click to close)</summary>
    Discuss the definition of (1) LLMs as agents, (2) tool augmentation, (3) reasoning and planning, (4) grounding.
  </details>
