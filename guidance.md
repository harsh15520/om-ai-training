**AI Engineering Training Plan** ke baare mein document (`AI-Engineering-Training-Plan 1 4.pdf`) aur orientation meeting (`latest_orientation`) mein jo bhi baatein batai gayi hain, unka poora detail neeche diya gaya hai:
 
---
 
### 1. Program Overview aur Philosophy
* **Target Audience & Purpose:** Ye plan khas karke naye **AI Engineering Interns** ke liye design kiya gaya hai [1]. Iska goal kisi ko zero AI background se is level tak lana hai jahan wo company ke system architectures padh sakein, workflows samajh sakein, aur Claude Code ki madad se real tasks implement kar sakein [1].
* **Duration & Structure:** Ye lagbhag **8–12 weeks** ka structured roadmap hai jisme total **10 project-gated phases (Phase 0 se Phase 9)** hain [1].
* **Core Philosophy:** Is training ka teen main pillars par focus hai:
  1. **Build to learn:** Sirf seekhna ya dekhna nahi hai, har phase ke end mein ek chota **"prove it" build/checkpoint** poora karna zaroori hai [1, 2].
  2. **Specify before you generate:** Code likhwane se pehle 1-paragraph architecture/plan sketch karna hoga [1, 3].
  3. **Own correctness:** AI (Claude Code) sirf code likhta hai, lekin architecture, plan, aur code sahi hai ya nahi — iski zimmedari human engineer ki hai [1, 4].
* **Orientation Meeting Context:** Pramod aur Deepti ne meeting mein bataya ki ye training steps/sheet daily tasks ke saath parallelly 1–2 weeks ke execution ke hisab se chalani hai taaki team members basic concepts (RAG, vector databases, fine-tuning, models, agents) ko ratne ki bajaye sahi se samajh sakein [5-8].
 
---
 
### 2. Phase-by-Phase Roadmap Details
 
* **Phase 0: Setup & Mindset (2–3 days)**
  * **Topics:** Python 3.11+, VS Code, Git (clone, branch, commit, push, PR) setup karna [4].
  * **Checkpoint:** Repository setup karna, branch banana, "hello world" Python script commit karke Pull Request (PR) open karna [9].
 
* **Phase 1: Python Foundations + OOP (1 week)**
  * **Topics:** Python syntax, data structures (lists, dicts, tuples), Object-Oriented Programming (classes, inheritance, `__init__`), NumPy, aur Pandas [9, 10].
  * **Checkpoint:** Inheritance ke saath ek Class likhna (jaise `BankAccount` ya `Task`) aur Pandas se CSV file load karke summary stats nikalna [10].
 
* **Phase 2: ML Fundamentals & Core Terminology (1–1.5 weeks)**
  * **Topics:** Supervised vs unsupervised learning, train/test split, overfitting/underfitting, bias/variance, linear regression, aur embeddings ki intuition [11, 12].
  * **Checkpoint:** Short doc ya Loom video ke dwara team ko explain karna ki overfitting, train/test split, aur embeddings kya hote hain [13].
 
* **Phase 3: Deep Learning, In Depth (2 weeks)**
  * **Topics:** Neurons, activation functions, forward pass, backpropagation, training loop, PyTorch basics, aur Andrej Karpathy ki "Zero to Hero" series [3, 13-15].
  * **Checkpoint:** Karpathy ke `micrograd` aur `makemore` exercises se tiny neural net aur character-level model scratch se build karna [14].
 
* **Phase 4: LLM Basics → Architecture → How They Work (1.5–2 weeks)**
  * **Topics:** Tokenization, Transformer architecture, self-attention (Q, K, V), pretraining vs fine-tuning, inference knobs (temperature, top-p, context window), aur hallucinations [16].
  * **Checkpoint:** Whiteboard ya diagram par Transformer data flow (raw text → tokens → embeddings → attention → output) draw karke explain karna [17].
 
* **Phase 5: Working With LLMs in Practice (1 week)**
  * **Topics:** LLM APIs call karna, prompt engineering (system prompts, JSON output), RAG (Retrieval-Augmented Generation) pipeline, aur Vector Databases (FAISS / Chroma) [17, 18].
  * **Checkpoint:** Internal docs ya PDFs ke saath grounding karke ek chota RAG demo build karna [18].
 
* **Phase 6: Frameworks, Agents & Multi-Agent (LangGraph) (2 weeks)**
  * **Topics:** LangChain basics, ReAct agent pattern, LangGraph state graphs (nodes, edges, checkpoints), aur Multi-Agent architectures (Supervisor vs Network patterns) [19, 20].
  * **Checkpoint:** Supervisor agent ke saath 2–3 worker agents wala LangGraph multi-agent system build karna [20].
 
* **Phase 7: Serving Models with FastAPI (1 week)**
  * **Topics:** REST API basics, FastAPI routes, Pydantic validation models, async programming, aur Docker containerization [21].
  * **Checkpoint:** Phase 6 ke agent ko FastAPI endpoint mein Pydantic validation ke saath wrap karna aur Dockerfile se containerize karna [22].
 
* **Phase 8: Architecture Thinking + Building With Claude Code (~3–4 days / ongoing)**
  * **Topics:** Internal project architectures padhna, data flow samajhna, Claude Code ko clear specs dena, aur generated code ko critically review karna [23, 24].
  * **Checkpoint:** Kisi realistic internal task ka architecture plan khud likhna, Claude Code se implement karwana, aur team ko walk-through dena [24].
 
* **Phase 9: AI Security: Grounding, Prompt Injection & Backend Validation (1 week)**
  * **Topics:** Direct vs Indirect prompt injection, system prompt vs security boundary, backend input/output validation, Pydantic schemas, aur OWASP Top 10 for LLM Applications [25-27].
  * **Checkpoint:** API mein Pydantic input validation add karna, privileged actions par backend rule lagana, aur indirect injection par threat-model note likhna [26].
 
---
 
### 3. Final Capstone Graduation Project & Key Resources
* **Capstone Project:** Graduation ke liye trainee ko ek end-to-end system build karna hota hai: **FastAPI service** jo ek **LangGraph multi-agent workflow** ko expose karti ho, jo documents par **RAG-based answers** de, **Pydantic input validation** ho, aur **prompt injection protection** guardrails lage hon [28].
* **Anchor Resources:**
  * Andrej Karpathy (*Zero to Hero*), StatQuest (Josh Starmer), 3Blue1Brown, Anthropic Prompt Docs, Official LangGraph Docs, FastAPI Tutorial, aur OWASP Top 10 for LLM Applications (2025) [14, 15, 19, 23, 27, 29].
* **Two Core Habits:**
  * Har phase ke end mein build checkpoint zaroor poora karna [2, 30].
  * Claude Code se code generate karwane se pehle hamesha architecture/plan sketch karna [3, 30].
 
---