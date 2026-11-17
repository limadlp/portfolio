# Dangeles Lima — Software Developer & Applied AI Engineer

This portfolio brings together selected software development projects, with a focus on Flutter mobile development and applied AI engineering. My mobile work includes apps built with Flutter and Dart, apps published on Google Play, and projects involving offline support, local storage, and automated testing. In applied AI, I build agents, orchestrate LLM workflows, and evaluate their performance. Each project includes a brief description of what I built and a link to the app or source code.

[View all repositories](https://github.com/limadlp) · [LinkedIn](https://www.linkedin.com/in/dangeles-lima/)

## Selected Projects

| Project | Area | Engineering focus |
| --- | --- | --- |
| [Lexicon](#lexicon--agent-orchestration-for-book-translation) | Applied AI | Parallel LLM workflows, shared glossary, and translation evaluation |
| [Especialistas](#especialistas--rag-for-personal-libraries) | Applied AI | Hybrid search over PDFs and EPUBs, with answers linked to source passages |
| [Entre Languages](#entre-languages--ai-powered-language-practice) | Applied AI | Language practice with concurrent character dialogue and writing feedback |
| [Practical Chord Transposer](#practical-chord-transposer) | Flutter | Published Android app with a custom chord editor and keyboard |
| [Travel Tech](#travel-tech--corporate-expense-management) | Flutter | Offline-first app with Drift, BLoC, and a reusable design system |
| [Practical Debt Control](#practical-debt-control) | Flutter | Published Android app for tracking debts and payments |

## Flutter Apps

### [Practical Chord Transposer](https://play.google.com/store/apps/details?id=com.axdtechnology.chordtransposer)

A Flutter app for Android with a custom chord keyboard and editor. Musicians can transpose an entire progression by semitones, then save or share it.

<details>
<summary>Screenshots</summary>

<img src="https://raw.githubusercontent.com/limadlp/limadlp.github.io/master/img/chord-transposer/chord-editor.png" alt="Chord editor with a C–G–Am–F progression" height="360"> <img src="https://raw.githubusercontent.com/limadlp/limadlp.github.io/master/img/chord-transposer/transposed-chords.png" alt="The same progression transposed up two semitones to D–A–Bm–G" height="360">

</details>

[Download on Google Play](https://play.google.com/store/apps/details?id=com.axdtechnology.chordtransposer).

### [Travel Tech — Corporate Expense Management](https://github.com/limadlp/travel_tech_test)

An offline-first corporate travel expense platform with a Flutter app, reusable design system, and lightweight Dart/Shelf backend. Built with Clean Architecture, Drift, BLoC, and Flutter Modular.

### [Practical Debt Control](https://play.google.com/store/apps/details?id=com.axdtechnology.debtcontrol)

A Flutter app for tracking debts and payments, published on Google Play.

<details>
<summary>Screenshots</summary>

<img src="https://play-lh.googleusercontent.com/uezSeu3ZC1QGKl2yZULtvmlpyfUhdtZIifSxyxrCtBOteoMz4HjOtVQ_NpyRi904lw=w1244-h973-rw" height="400">   <img src="https://play-lh.googleusercontent.com/x7agnslYDLSfcpBeRvaB6XvL_9JN__joPkVJWyDcUygbM6lGy0X4rFXvpzVeHGNfZ2k=w1244-h973-rw" height="400">   <img src="https://play-lh.googleusercontent.com/XDaizKYmOUcOUHlPiw60txny0wFO-Pxf-QowlYaB2_Dpbmfhls1urPZGEevjEYTb1lKy=w1244-h973-rw" height="400">
<img src="https://play-lh.googleusercontent.com/EgfCGL9GbKBkYKVX1OD84Y5uaFI1re9ZgOeq3D-tMdXTDRKMi8EgYQC0z3X4ttVBfg=w1244-h973-rw" height="400">
<img src="https://play-lh.googleusercontent.com/hnBJoQMQRcifeJng0LHxvSR9xrsH-IYrjd7KBbKN4dXAgzKGClKlAV2DzfzYwPOV5A=w1244-h973-rw" height="400">

</details>

[Download on Google Play](https://play.google.com/store/apps/details?id=com.axdtechnology.debtcontrol).

### [QueroMais Vegano](https://github.com/limadlp/queromaisvegano)

An online store app built with Provider and Firebase, featuring Cielo API integration.

<details>
<summary>Screenshots</summary>

<img src="https://github.com/limadlp/queromaisvegano/raw/master/img/Screenshot_001.png" height="400"> <img src="https://github.com/limadlp/queromaisvegano/raw/master/img/Screenshot_003.png" height="400"> <img src="https://github.com/limadlp/queromaisvegano/raw/master/img/Screenshot_002.png" height="400"> <img src="https://github.com/limadlp/queromaisvegano/raw/master/img/Screenshot_004.png" height="400">

</details>

[View source code](https://github.com/limadlp/queromaisvegano).

### [Practical House Manager](https://github.com/limadlp/practical_house_manager)

An app for coordinating household expenses and organization between housemates. It uses WebSockets, a Go API, Flutter Modular, MVVM with the Repository pattern, and MobX. Work in progress.

[Flutter app](https://github.com/limadlp/practical_house_manager) · [Go API](https://github.com/limadlp/house-manager-api)

### More Flutter Projects

- [Movie App — GetX and REST API](https://github.com/limadlp/app_filmes_getx)
- [To-Do List — Provider, SQFLite, and modular architecture](https://github.com/limadlp/todolist_provider)
- [Raro Technical Test — responsive financial UI, BLoC, and automated tests](https://github.com/limadlp/raro_test)
- [Rispar Mobile Developer Test — credit simulator with responsive UI, API calls, MVVM, and Provider](https://github.com/limadlp/rispar_simulator)

#### Flutter Minigames

- [Flappy Bird](https://limadlp.github.io/flappy)
- [Mario](https://limadlp.github.io/mario)
- [Pong](https://limadlp.github.io/pong)
- [Brick Breaker](https://limadlp.github.io/brickbreaker/index.html#/)

#### Flutter Sandbox

A collection of study projects covering Clean Architecture, testing, state management, packages, and related topics.

- [Flutter Sandbox](https://github.com/limadlp/flutter-sandbox)

---

## AI Engineering

### [Lexicon — Agent Orchestration for Book Translation](https://github.com/limadlp/lexicon-agent-orchestration)

I built a Python pipeline that translates EPUB and Markdown books into Brazilian Portuguese. It processes chapters concurrently using a shared glossary to keep terminology and character references consistent. After consolidating glossary updates, it revises only chapters affected by conflicts.

I implemented interchangeable orchestration engines using asyncio, LangGraph, and Google ADK, and used *The Wonderful Wizard of Oz* to evaluate terminology consistency across chapters.

[Source code](https://github.com/limadlp/lexicon-agent-orchestration)

### [Especialistas — RAG for Personal Libraries](https://github.com/limadlp/especialistas-rag)

I built a local app for asking questions about PDF and EPUB collections. Each assistant has its own library, instructions, and conversation history. Citations in each answer open the supporting passage in the source document.

The Python and FastAPI backend combines multilingual E5 embeddings in Qdrant with BM25 keyword search. An LLM reranks passages and can request a follow-up search when evidence is missing. The project includes evaluations for retrieval, answer accuracy, and citations.

[Source code](https://github.com/limadlp/especialistas-rag)

### [Entre Languages — AI-Powered Language Practice](https://github.com/limadlp/entre-languages)

I built a web app for practicing English, Brazilian Portuguese, Spanish, and Mandarin Chinese through conversations with fictional AI characters. An optional language critic suggests more natural wording and explains the changes in the learner's chosen language.

A Python orchestrator runs the character and critic concurrently with asyncio. FastAPI streams each result to the React frontend as it completes, so learners can keep chatting while feedback is pending.

[Source code](https://github.com/limadlp/entre-languages)

## Web Frontend

- [Pizzashop dashboard](https://github.com/limadlp/pizzashop-web) — Vite and React
- [Task manager](https://github.com/limadlp/tarefas-nextjs) — React and Next.js
- [Developer support manager](https://github.com/limadlp/devcontrole-nextjs) — React and Next.js

## Backend & APIs

### Go

- [House Manager API](https://github.com/limadlp/house-manager-api)
- [Go Sandbox](https://github.com/limadlp/go-sandbox)

### Node.js

Study projects for a forum built with DDD, Clean Architecture, and NestJS:

- [Clean DDD](https://github.com/limadlp/04-clean-ddd)
- [NestJS with Clean Architecture](https://github.com/limadlp/05-nest-clean)

## Computational Simulation and Data Analysis

### [Computational Neuroscience](https://github.com/limadlp/NeuroComp)

#### [C++ Classes](https://github.com/limadlp/NeuroComp/tree/main/Cpp)

I developed a reusable computational interface for multiple network structures, neuronal dynamics, and synapse models. Its core is divided into two classes:

- `rede.h`, containing network structures;
- `dinamica.h`, containing neuronal dynamics and synapse models.

The [repository includes examples](https://github.com/limadlp/NeuroComp/tree/main/Cpp) using one-dimensional, square, and hierarchical modular networks, as well as integrate-and-fire, Izhikevich, and simplified Levina–Herrmann–Geisel models.

#### [Neuron Models in Julia](https://github.com/limadlp/NeuroComp/tree/main/Julia)

- [Leaky integrate-and-fire](https://github.com/limadlp/NeuroComp/blob/main/Julia/LeakyIF.ipynb)
- [Exponential integrate-and-fire](https://github.com/limadlp/NeuroComp/blob/main/Julia/ExpoIF.ipynb)
- [Hodgkin–Huxley](https://github.com/limadlp/NeuroComp/blob/main/Julia/HxHuxley.ipynb)

#### [Neuronal Avalanches — Data Analysis](https://github.com/limadlp/NeuroComp/blob/main/DataScience/Avalanche.ipynb)

A short [Python analysis](https://github.com/limadlp/NeuroComp/blob/main/DataScience/Avalanche.ipynb) of data from a simulation of 1,024 leaky integrate-and-fire neurons on a square network. It examines the neuronal avalanche distribution and its power-law behavior through a log-log plot.

---

### [Luck vs Talent](https://github.com/limadlp/LuckvsTalent)

A C++ and Python simulation exploring the relationship between intelligence and financial success, based on an [agent-based model](https://arxiv.org/pdf/1802.07068.pdf). My version removes the spatial environment and samples events probabilistically at each iteration.

[View details and source code](https://github.com/limadlp/LuckvsTalent).

---

### [Arduino Biofeedback](https://github.com/limadlp/Biofeedback)

Circuits and code for capturing biosignals from Arduino in real time. [View the project](https://github.com/limadlp/Biofeedback).

---

### [Satellite Orbital Dynamics](https://github.com/limadlp/OrbitalDynamics)

Fortran code used in a computational simulation study of satellite orbital transfers. The work proposes non-impulsive maneuvers based on a differentiated Hohmann equation, producing a semi-analytical model for transfers between nearby orbits.

---

### [Blackjack with Neuroevolution](https://github.com/limadlp/Blackjack)

An AI agent built to play Blackjack using neural networks and genetic algorithms.

[View details and source code](https://github.com/limadlp/Blackjack).

---

### [Pokémon Dataset](https://github.com/limadlp/Pokemon/blob/master/Pokemon3.ipynb)

Exploratory analysis of a [Pokémon dataset](https://www.kaggle.com/abcsds/pokemon) available on [Kaggle](https://www.kaggle.com/).

[View the Jupyter notebook](https://github.com/limadlp/Pokemon/blob/master/Pokemon3.ipynb).
