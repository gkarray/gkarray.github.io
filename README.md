# About me
I am a **Data Science Engineer** with a Master’s degree from **EPFL**. I have strong programming skills and a deep fascination with how intelligence works—both in machines and in ourselves.

### I build to solve
I am at my best when I am building digital solutions for complex, real-world problems. While I value high-level theory, I am primarily driven by the satisfaction of turning a messy challenge into a reliable piece of software. I have cultivated a versatile skill set across the entire technical stack. I am equally comfortable designing system architectures, developing software, engineering data pipelines, or training machine learning models. My focus is always on selecting the right tool for the specific problem and its constraints, whether that requires a classical machine learning approach, a state-of-the-art Large Language Model, or more experimental solutions like Spiking Neural Networks.

### I study the mechanics of the mind
I see Artificial Intelligence as a way to reverse-engineer how we think. My technical designs are often informed by insights from philosophy, neuroscience, and cognitive science. This curiosity led me to **Intel Labs**, where I developed neuromorphic systems to explore brain-inspired computing. I continue this exploration through my **EmbodiedAI Gymnasium** project, a sandbox for benchmarking diverse cognitive models.

Lately, I have been immersed in _Active Inference_. Theoretically, I am compelled by how it marries Bayesian and Enactive theories of mind. In practice, I find it a more principled framework for designing agents than most contemporary "agentic" systems, and it also provides a promising path toward solving fundamental challenges like online continual learning and transfer learning.

### I believe in collective intelligence
Intelligence isn’t restricted to a single brain or chip; it happens between us, too. I feel a strong mission to use technology to enhance this collective intelligence, specifically through Digital Democracy. I am interested in how digital tools can help us think, deliberate, and solve problems more effectively as a society. This drive led to my research at the **University of Zürich**, where I used LLMs for Argument Mining to map argumentation patterns in discourse. It also powers my current work on the **MapOfBelief** project, an application designed to visualize the structural dynamics and shifting beliefs within online communities.

### In short...
I’m a builder who likes to think, and a thinker who loves to build. Whether I am developing a complex piece of software or exploring the latest in brain-inspired computing, I’m always looking for ways to bridge the gap between complex theory and practical, human-centric solutions.


# Open projects
### ArdhiPilot: AgriTech platform
* **Vision:** A startup project I am co-founding as the AI and Data Science Lead. We are building a real-time field monitoring platform designed to put data-driven insights directly into the hands of farmers. The system integrates user-reported field logs (activities, crop types, historical interventions) with multi-modal data—including Sentinel-2 multispectral imagery, meteorological streams, and IoT soil sensors—to provide actionable crop health diagnostics and predictive yield forecasts.
* **Engineering:** 
    * **Backend Infrastructure:** Developed a backend system with secure authentication and a relational database schema designed to manage complex user-reported field activities, crop logs, and historical data.
    * **Geospatial Data System:** Engineered a spatial database to perform high-performance geographic indexing and multi-temporal querying across satellite data and field geometries.
    * **Remote Sensing Pipelines:** Implemented automated workflows to ingest Sentinel-2 multispectral imagery and transform raw bands into calibrated vegetation indices (e.g., NDVI) for real-time vigor monitoring.
    * **Ongoing development:**
        * **Multi-Modal Integration:** Fusing meteorological data with satellite observations to provide environmental context for vegetation health patterns.
        * **Semantic Segmentation:** Training Computer Vision models for automated land use and land cover (LULC) classification and field boundary delineation.
        * **Predictive Modeling:** Building forecasting engines to estimate harvest yields based on historical trends and current health markers.
* **Topics:** Backend Software Engineering, Data Engineering, Machine Learning, Computer Vision, Geospatial Data Analysis, IoT
* **Link:** [ArdhiPilot website](https://ardhipilot.com/)


### ZettelkastenAssistant: LLM-powered ObsidianMD plugin
* **Vision:** A plugin that transforms personal research notes into a structured knowledge system. The project focuses on two core capabilities: automatically ingesting unstructured markdown notes into a knowledge graph and leveraging that ontology to derive new insights and assist in writing articles and research papers.
* **Engineering:** 
    * **Plugin Architecture:** Developed the core ObsidianMD plugin using TypeScript, creating a high-performance bridge between the local markdown environment and remote/local LLM backends (vLLM and Google AI API).
    * **Knowledge Graph Ingestion:** Built an automated extraction pipeline using LangChain.js that identifies entities and relationships within notes to populate a Neo4j graph, effectively mirroring the vault's structure in a queryable database.
    * **Ongoing development:**
        * **Graph-RAG Retrieval:** Developing a real-time retrieval system that traverses the knowledge graph to provide context-aware suggestions and ideas as the user writes.
        * **Agentic Synthesis Workflows:** Implementing multi-agent systems to analyze the graph, identify hidden connections across distant note clusters, and propose structured outlines for complex papers.
        * **Dynamic Ontology Evolution:** Designing logic that allows the system to suggest new node types or relationship categories as the research vault grows, ensuring the underlying schema adapts to the user's study.
* **Stack:** TypeScript, LangChain.js, Neo4j, Google AI API, vLLM, ObsidianMD
* **Topics:** Natural Language Processing, Large Language Models (LLMs), Knowledge Graphs, Retrieval Augmented Generation (RAG), Agentic Systems, Zettelkasten

### MapOfBelief: Visualization app for dynamics of beliefs in online discourse
* **Vision:** An application designed to visualize the "topology" of human beliefs by inferring them from raw discourse. By detecting patterns in how people argue, the system extrapolates underlying belief systems and maps them across multiple scales—from individual claims to shared community narratives. The project aims to track the dynamics of these beliefs over time, providing insights into how they shift or solidify through online debate.
* **Engineering:** 
    * **Argument Mining Engine:** Developed an LLM-based pipeline to extract atomic claims from noisy social media text and identify the logical relationships between them, specifically focusing on support and contradiction.
    * **Multi-Scale Knowledge Graph:** Designed a Neo4j schema capable of transitioning between different levels of granularity: mapping how individual claims link together to form personal belief systems, and how those systems aggregate into collective community narratives.
    * **Ongoing development:**
        * **Temporal Dynamics Mapping:** Implementing logic to track the evolution of specific argument clusters over time to analyze how beliefs change in response to real-world events or sustained discourse.
        * **Interactive Graph Visualization:** Developing a high-performance D3.js and React interface to navigate massive belief networks, allowing users to toggle between abstract graph structures and the actual raw text that informs them.
        * **Polarization Analysis:** Building analytical tools to quantify "echo chamber" effects and identify the central nodes of logical or rhetorical contention within online sub-cultures.
* **Stack:** Python, FastAPI, LangChain, Neo4j, Google AI API, vLLM, TypeScript, React, D3.js
* **Topics:** Natural Language Processing, Large Language Models (LLMs), Knowledge Graphs, Retrieval Augmented Generation (RAG), Agentic Systems, Argumentation Theory, Interactive Large Scale Graph Visualization

### EmbodiedAI Gymnasium: Sandbox for cognitive models
* **Vision:** A research repository for benchmarking and comparing diverse perception and control paradigms—ranging from classical robotics and deep learning to brain-inspired models. The project provides a unified sandbox to test how biologically plausible architectures, such as Active Inference and Spiking Neural Networks (SNNs), perform on embodied AI tasks. Ultimately, I am using this environment to develop the "cognitive engine" for a future video game project where gameplay revolves around a human player cooperating with a SNN implementation of an Active Inference agent to solve complex puzzles.
* **Engineering:** 
    * **Infrastructure & Interface:** Architected a modular interface between the OpenAI Gymnasium ecosystem and diverse modeling frameworks, including PyTorch, BindsNet (SNNs), and PyMDP (Active Inference), and integrated Visdom to enable live visualization and real-time telemetry of internal state variables and model performance as the simulation runs.
    * **CartPole Multi-Paradigm Benchmark:** Successfully implemented and compared five distinct solutions to the CartPole problem: Heuristics, Model Predictive Control (MPC), Deep Reinforcement Learning, Spiking Neural Networks, and Active Inference.
    * **Ongoing development:**
        * **High-Dimensional Control & SLAM:** Expanding simulations from 2D to 3D environments to benchmark diverse solutions for Simultaneous Localization and Mapping (SLAM) and complex spatial navigation.
        * **Multi-Modal Sensory Fusion:** Developing computer vision pipelines and sensor-fusion layers to test how different cognitive models integrate high-frequency visual and tactile data for real-time decision-making.
        * **Online Continual & Transfer Learning:** Investigating synaptic plasticity and Bayesian updating rules to enable agents to continually learn new tasks in real-time and transfer knowledge to novel environments without catastrophic forgetting.
        * **Social Emergence & AI Societies:** Implementing multi-agent scenarios to study the emergence of cooperation and coordination, aiming to develop "societies" of agents that mirror human-like interaction and functional dynamics in complex environments.
* **Stack:** Python, Gymnasium, MuJoCo, PyTorch, BindsNet, PyMDP, Visdom
* **Topics:** Embodied Artificial Intelligence, Robotics, Machine Learning, Control Theory, Computer Vision, SLAM, Sensor Fusion, Cogntive Modelling, Spiking Neural Networks, Active Inference

# Publications
<dl>

<dt>Assessing Reliability and Political Bias In LLMs’ Judgements of Formal and Material Inferences With Partisan Conclusions</dt>
<dd>Reto Gubelmann, Ghassen Karray</dd>
<dd>ACL 2025</dd>
<dd>Link: https://aclanthology.org/2025.acl-long.1450/</dd>

<dt>Identifying open-texture in regulations using LLMs</dt>
<dd>Clement Guitton, Reto Gubelmann, Ghassen Karray, Simon Mayer & Aurelia Tamò-Larrieux</dd>
<dd>Artificial Intelligence and Law 2025</dd>
<dd>Link: https://link.springer.com/article/10.1007/s10506-025-09450-0</dd>

<dt>Dynamic graph exploration by interactively linked node-link diagrams and matrix visualizations</dt>
<dd>Michael Burch, Kiet Bennema ten Brinke, Adrien Castella, Ghassen Karray, Sebastiaan Peters, Vasil Shteriyanov & Rinse Vlasvinkel </dd>
<dd>Visual Computing for Industry, Biomedicine, and Art 2021</dd>
<dd>Link: https://link.springer.com/article/10.1186/s42492-021-00088-8</dd>

</dl>