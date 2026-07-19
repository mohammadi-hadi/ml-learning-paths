# ML Learning Paths

**The best machine learning courses on the internet, organized into five career paths — ML scientist, ML engineer, LLM engineer, data engineer, and data scientist — with an honest opinion about what to take, in what order, and what to skip.**

![Last reviewed](https://img.shields.io/badge/last_reviewed-July_2026-1E3A5F)
![Links checked weekly](https://img.shields.io/badge/links-checked_weekly-1E3A5F)
[![License: MIT](https://img.shields.io/badge/license-MIT-1E3A5F)](LICENSE)

There are hundreds of ML course lists. Most of them are 200-item link dumps that answer the wrong question. The question is never *"what courses exist?"* — it is *"I want this job; what do I do next?"*

This guide answers the second question. I'm a machine learning scientist (PhD in NLP, now building production LLM and ranking systems in industry), and these are the courses I actually point people to when they ask where to start. Every path is ordered, every entry says *why it's there*, and every path can be completed for free.

## Contents

- [How to use this guide](#how-to-use-this-guide)
- [Which path is yours?](#which-path-is-yours)
- [Foundations (everyone)](#foundations-everyone)
- [Path 1 — ML Scientist](#path-1--ml-scientist)
- [Path 2 — ML Engineer](#path-2--ml-engineer)
- [Path 3 — LLM / AI Engineer](#path-3--llm--ai-engineer)
- [Path 4 — Data Engineer](#path-4--data-engineer)
- [Path 5 — Data Scientist](#path-5--data-scientist)
- [A note on certificates](#a-note-on-certificates)
- [Contributing](#contributing)

## How to use this guide

1. **Pick one path.** The roles genuinely differ; studying "a bit of everything" is the slowest route to any of them.
2. **Do the stages in order.** Each stage assumes the previous one. Skipping foundations to get to the shiny part is the most common mistake I see.
3. **Build after every stage.** A course you didn't apply is a course you'll forget. Each path ends with a "prove it" project — that project, on your GitHub, is worth more than any certificate.
4. **Free first.** Where a paid and a free option are equally good, the free one is listed. Coursera courses can be audited for free (certificates cost money; the knowledge doesn't).

Rough time investment: foundations 1–2 months, then 4–8 months per path at ~10 hours/week. Anyone selling you a shortcut is selling you something.

## Which path is yours?

| Path | You spend your days | Typical entry point |
|---|---|---|
| [ML Scientist](#path-1--ml-scientist) | Designing models and experiments, reading papers, proving a method works | Quantitative degree, or strong math + patience |
| [ML Engineer](#path-2--ml-engineer) | Getting models into production and keeping them there | Software engineering background |
| [LLM / AI Engineer](#path-3--llm--ai-engineer) | Building products on top of LLMs: RAG, agents, evaluation | Software engineering, less math required |
| [Data Engineer](#path-4--data-engineer) | Building the pipelines and warehouses everyone else depends on | Software engineering or analytics |
| [Data Scientist](#path-5--data-scientist) | Analysis, experiments (A/B tests), models that inform decisions | Statistics, economics, any analytical field |

Boundaries blur in real companies — I have done all five in a single job — but train for one center of gravity.

## Foundations (everyone)

Skip individual items you already have. Do not skip the math because it looks optional; it becomes the ceiling on everything later.

| Course | Provider | Cost | Why this one |
|---|---|---|---|
| [Essence of Linear Algebra](https://www.3blue1brown.com/topics/linear-algebra) | 3Blue1Brown | Free | The geometric intuition (what a matrix *does*) that formula-first courses never give you. Watch it before any formal course. |
| [Mathematics for Machine Learning](https://mml-book.github.io/) | Deisenroth, Faisal, Ong | Free (book) | The one reference that covers exactly the linear algebra, calculus, and probability ML needs — no more. Companion [Coursera specialization](https://www.coursera.org/specializations/mathematics-machine-learning) if you want structure. |
| [CS50's Introduction to Programming with Python](https://cs50.harvard.edu/python/) | Harvard | Free | If you can't yet write clean Python from scratch, this is the fastest respectable route. |
| [Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction) | DeepLearning.AI / Stanford (Andrew Ng) | Free to audit | Still the best first contact with ML: regression → classification → trees → basic neural nets, with the right amount of math. |
| [Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course) | Google | Free | Compact, exercise-driven second pass; good litmus test that the fundamentals stuck. |
| [Kaggle Learn](https://www.kaggle.com/learn) | Kaggle | Free | Micro-courses (pandas, feature engineering, model validation) to convert theory into working code fast. |

## Path 1 — ML Scientist

The research-leaning role: you design methods, run experiments, and are accountable for *whether the model is actually good*. The math bar is the highest of the five paths; so is the reading load. This is my own path, and the honest summary is: depth beats breadth, and implementation beats both.

| Stage | Course | Provider | Cost | Why this one |
|---|---|---|---|---|
| 1. Theory | [CS229: Machine Learning](https://cs229.stanford.edu/) | Stanford | Free | The canonical rigorous ML course. Where Andrew Ng's Coursera course shows you the moves, CS229 proves them. |
| 2. Deep learning | [Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning) | DeepLearning.AI | Free to audit | Systematic DL foundations: backprop, CNNs, sequence models, tuning. |
| 2. Deep learning (alt) | [Dive into Deep Learning (d2l.ai)](https://d2l.ai/) | Zhang, Lipton, Li, Smola | Free | Interactive book used at 500+ universities; every concept comes with runnable code. Pick this if you learn by implementing. |
| 3. From scratch | [Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html) | Andrej Karpathy | Free | Build backprop, then GPT, from raw Python. The single highest-signal-per-hour resource on this page. |
| 4. Vision | [CS231n: Deep Learning for Computer Vision](https://cs231n.stanford.edu/) | Stanford | Free | The classic treatment of CNNs and modern vision; the assignments are the point. |
| 4. Language | [CS224n: NLP with Deep Learning](https://web.stanford.edu/class/cs224n/) | Stanford | Free | From word vectors to transformers. If you touch text (increasingly: everyone), take it. |
| 5. LLMs deeply | [CS336: Language Modeling from Scratch](https://stanford-cs336.github.io/spring2025/) | Stanford | Free | Build a full LLM pipeline — tokenizer, architecture, training, alignment — yourself. The 2020s equivalent of "write your own compiler". |
| 6. Fast survey | [MIT 6.S191: Introduction to Deep Learning](https://introtodeeplearning.com/) | MIT | Free | Annually refreshed lectures; efficient way to keep the survey-level view current. |
| Optional: RL | [Spinning Up in Deep RL](https://spinningup.openai.com/en/latest/) → [David Silver's RL course](https://www.davidsilver.uk/teaching/) → [CS285: Deep RL](https://rail.eecs.berkeley.edu/deeprlcourse/) | OpenAI / DeepMind / Berkeley | Free | In that order: pragmatic intro → classic theory → research depth. RL matters more now that RLHF/GRPO sit inside every LLM stack. |

**If you only take three:** Zero to Hero, CS229, CS224n.

**Prove it:** re-implement one paper relevant to your target area and reproduce its headline number (or document honestly why you couldn't — negative reproductions are respected). Put the code, the plots, and a short write-up in one repository.

**The habit that matters:** read one paper properly per week and skim ten. [Hugging Face Papers](https://huggingface.co/papers) is a good daily feed.

## Path 2 — ML Engineer

The role that turns a model into a system: serving, monitoring, retraining, and the unglamorous 90% of ML that isn't modeling. Demand for this profile exceeds supply more than for any other path here. Prerequisite: solid software engineering and the Foundations block.

| Stage | Course | Provider | Cost | Why this one |
|---|---|---|---|---|
| 1. ML refresher | [Machine Learning Zoomcamp](https://github.com/DataTalksClub/machine-learning-zoomcamp) | DataTalksClub | Free | Four-month practical course ending in deployment, with an active community and homework that gets reviewed. |
| 2. The mindset | [Made With ML](https://madewithml.com/) | Goku Mohandas | Free | Design → develop → deploy → iterate on one project, with production-quality code throughout. The best single introduction to *ML as engineering*. |
| 3. MLOps | [MLOps Zoomcamp](https://github.com/DataTalksClub/mlops-zoomcamp) | DataTalksClub | Free | Experiment tracking, orchestration, deployment, monitoring — the concrete toolchain, hands-on. |
| 4. Systems design | [CS 329S: ML Systems Design](https://stanford-cs329s.github.io/) | Stanford (Chip Huyen) | Free | The reasoning layer above the tools: data distribution shift, feature stores, online evaluation. Lecture notes read like a good book (Chip Huyen later turned them into one). |
| 5. Full picture | [Full Stack Deep Learning](https://fullstackdeeplearning.com/) | FSDL | Free | From problem framing to shipped product, including the LLM era. Strong on what breaks in the real world. |
| 6. Production practice | [Machine Learning in Production](https://www.coursera.org/learn/introduction-to-machine-learning-in-production) | DeepLearning.AI | Free to audit | Andrew Ng on scoping, data pipelines, and deployment patterns — a compact complement to the Zoomcamps. |
| 7. Under the hood | [10-714: Deep Learning Systems](https://dlsyscourse.org/) | CMU | Free | Build your own autograd framework and GPU kernels. Optional but transformative: after this, no framework is a black box. |

**If you only take three:** Made With ML, MLOps Zoomcamp, CS 329S.

**Prove it:** take a model — even a boring one — and ship it: containerized API, CI that runs tests, monitoring dashboard, one-command redeploy, and a README explaining the design trade-offs. A boring model served excellently beats a SOTA notebook every time. Interviewers open the repo; make the engineering the star.

## Path 3 — LLM / AI Engineer

The newest role: building products on top of foundation models — retrieval, agents, tool use, and above all evaluation. Less math than Path 1, more product judgment. It is also the path where courses age fastest, so favor sources that are actively maintained (everything below is).

| Stage | Course | Provider | Cost | Why this one |
|---|---|---|---|---|
| 1. Core | [Hugging Face LLM Course](https://huggingface.co/learn/llm-course) | Hugging Face | Free | Transformers, fine-tuning, and the HF ecosystem the whole field standardized on. Start here. |
| 2. The map | [LLM Course](https://github.com/mlabonne/llm-course) | Maxime Labonne | Free | The best-organized roadmap of the LLM landscape (fundamentals / scientist / engineer branches), with notebooks. Use it to see the whole territory. |
| 3. Prompting & patterns | [Prompt Engineering Guide](https://www.promptingguide.ai/) | DAIR.AI | Free | Prompting techniques with the papers behind them — a reference you'll return to, not a one-off read. |
| 4. Agents | [Hugging Face Agents Course](https://huggingface.co/learn/agents-course) | Hugging Face | Free | Function calling, agent frameworks, and evaluation of agentic systems, hands-on. |
| 4. Agents (frameworks) | [LangChain Academy](https://academy.langchain.com/) | LangChain | Free | Short courses on LangGraph and production agent patterns from the team that builds them. |
| 5. Applied patterns | [DeepLearning.AI Short Courses](https://www.deeplearning.ai/short-courses/) | DeepLearning.AI | Free | 1–2 hour courses on RAG, evaluation, fine-tuning, agents — built with the vendor teams. Cherry-pick per need. |
| 5. Vendor cookbooks | [Anthropic Courses](https://github.com/anthropics/courses) · [OpenAI Cookbook](https://cookbook.openai.com/) | Anthropic / OpenAI | Free | Working code for tool use, structured outputs, evaluation. Read cookbooks the way previous generations read framework docs. |
| 6. Understanding | [CS324: Large Language Models](https://stanford-cs324.github.io/winter2022/) | Stanford | Free | What's actually inside the model you're calling: capabilities, harms, data, scaling. The 2022 vintage shows its age on tooling, not on concepts. |
| 6. Frontier view | [CS25: Transformers United](https://web.stanford.edu/class/cs25/) | Stanford | Free | Rotating guest lectures from the people building frontier models; the cheapest way to hear the state of the art firsthand. |

**If you only take three:** HF LLM Course, HF Agents Course, plus the DeepLearning.AI short courses on RAG and evaluation.

**Prove it:** build a RAG or agent application on your own documents — with an evaluation harness. The eval set, the judge prompts, and the metrics table are what separate a professional from a demo. (Evaluation is the part of this stack most teams do worst; from my own work on LLM-as-judge evaluation, it is also the part interviewers probe hardest.)

## Path 4 — Data Engineer

The foundation everyone else stands on: ingestion, warehouses, transformation, streaming. Less hyped than the other paths and more consistently employable. Prerequisite: SQL and Python.

| Stage | Course | Provider | Cost | Why this one |
|---|---|---|---|---|
| 1. SQL, properly | [SQLBolt](https://sqlbolt.com/) → [Mode SQL Tutorial](https://mode.com/sql-tutorial) | SQLBolt / Mode | Free | Interactive basics, then analytical SQL (window functions, CTEs) on realistic data. Fluency here is non-negotiable. |
| 2. The core | [Data Engineering Zoomcamp](https://github.com/DataTalksClub/data-engineering-zoomcamp) | DataTalksClub | Free | The definitive free DE course: Docker, Terraform, orchestration, warehouse, Spark, Kafka, dbt — one cohort-based project. If you do one thing on this path, do this. |
| 3. Transformation | [dbt Learn](https://learn.getdbt.com/) | dbt Labs | Free | Official courses for the tool that defines the "analytics engineering" layer of the modern stack. |
| 4. Orchestration | [Astronomer Academy](https://academy.astronomer.io/) | Astronomer | Free | Airflow fundamentals from the company that maintains it. |
| 5. Streaming | [Confluent Developer](https://developer.confluent.io/) | Confluent | Free | Kafka courses and patterns from the source; the streaming equivalent of reading the manual, except good. |
| 6. Big data engines | [Databricks Learning](https://www.databricks.com/learn) | Databricks | Free tier | Spark fundamentals and lakehouse patterns. (For distributed data processing at scale, Spark is still the lingua franca.) |
| 7. Depth | [CMU 15-445: Database Systems](https://15445.courses.cs.cmu.edu/) | CMU | Free | How databases actually work: storage, indexing, query execution, transactions. The difference between using tools and understanding them. |

**If you only take three:** DE Zoomcamp, dbt Learn, CMU 15-445.

**Prove it:** an end-to-end pipeline on real public data (e.g., open transport or energy feeds): ingestion → warehouse → dbt models → dashboard, orchestrated, tested, with documented data-quality checks. Include one design decision you reversed and why — that's the part that reads as senior.

## Path 5 — Data Scientist

The analysis-and-inference role: experiments, causal questions, metrics, and models whose output is a *decision*, not an API. Statistics is the moat — plenty of people can fit a model; far fewer can tell you whether the effect is real.

| Stage | Course | Provider | Cost | Why this one |
|---|---|---|---|---|
| 1. Statistical intuition | [Seeing Theory](https://seeing-theory.brown.edu/) | Brown | Free | Interactive visual probability and statistics; fixes intuition before formalism. |
| 2. Core | [An Introduction to Statistical Learning](https://www.statlearning.com/) | James, Witten, Hastie, Tibshirani | Free (book + lectures) | The classic. Regression, classification, resampling, trees — with the statistical honesty ML courses often skip. Python and R editions. |
| 3. Practice | [Kaggle Learn](https://www.kaggle.com/learn) | Kaggle | Free | Pandas → visualization → ML micro-courses; fastest route from theory to working analysis. |
| 4. Structured program | [Google Advanced Data Analytics](https://www.coursera.org/professional-certificates/google-advanced-data-analytics) | Google / Coursera | Free to audit | If you want one guided end-to-end program (statistics, regression, ML, capstone), this is the strongest of the big-tech certificates. |
| 5. Causality & experiments | [Causal Inference for the Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html) | Matheus Facure | Free | A/B testing, diff-in-diff, IV, synthetic control — in Python, with humor. This material is what separates senior DS interviews from junior ones. |

**If you only take three:** Statistical Learning, the causality handbook, Kaggle Learn.

**Prove it:** one deep analysis of a dataset you care about, framed as a decision: a clear question, an honest experiment or causal design, effect sizes with uncertainty, and a recommendation. Write it up so a non-technical stakeholder could act on it. (In industry I've seen a single strong A/B-test write-up carry an interview.)

## A note on certificates

Hiring managers (I am sometimes one) generally read a CV in this order: what you built → where you worked/studied → *maybe* certificates. Courses are for acquiring skill, and the portfolio project at the end of each path is how the skill becomes visible. Pay for a certificate if your situation rewards it (visa paperwork, internal promotion process, structured motivation) — not because it "counts" by itself.

## Related guides

- [ml-summer-schools-europe](https://github.com/mohammadi-hadi/ml-summer-schools-europe) — ML summer schools in Europe: deadlines, funding, and how to get in
- [ai-masters-netherlands](https://github.com/mohammadi-hadi/ai-masters-netherlands) — every AI/DS master's programme in the Netherlands, with admissions and costs
- [modern-ai-engineering](https://github.com/mohammadi-hadi/modern-ai-engineering) — field notes on production LLM systems, one level deeper than the courses

## Contributing

Corrections and course suggestions are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md). The bar for adding a course is deliberately high: it must be the *best* option for a specific stage, not merely good.

## License

[MIT](LICENSE) — maintained by [Hadi Mohammadi](https://mohammadi.cv). Links are checked weekly by CI; content last reviewed July 2026.
