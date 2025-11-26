# Natural Language Processing (ITAI 2373)
**Student:** Chloe Tu  
**Program:** Articial Intelligence A.A.S

## 📖 Course Overview
This repository serves as a comprehensive portfolio of coursework, labs, and innovative projects completed during the **ITAI 2373 Natural Language Processing** course. The work documented here demonstrates a progression from foundational text processing to advanced applications in Neural Network architecture, Generative Adversarial Networks (GANs), Voice Technology, and Ethical AI design.

## 🛠 Skills & Technologies
* **Languages & Environments:** Python 3.x, Jupyter Notebooks
* **Key Libraries:** NLTK, Pandas, NumPy, Scikit-learn, TensorFlow/Keras
* **Core Competencies:**
    * **Text Preprocessing:** Tokenization, Stemming/Lemmatization, Stop-word removal, Regex cleaning.
    * **Modeling:** Artificial Neural Networks (ANNs), Seq2Seq models, Predictive Modeling.
    * **Concepts:** Vectorization (TF-IDF, Bag-of-Words), Backpropagation, Gradient Descent, GANs (Generator/Discriminator dynamics), POS Tagging.
    * **Soft Skills:** Ethical AI analysis, Technical storytelling, System design.

---

## 📂 Project & Lab Structure

### 🔹 Module 01: Introduction to NLP
* **File:** `NLP-in-Action-From-Pop-Culture-to-Processes_Chloe_Tu_ITAI_2373.pdf`
* **Description:** An introductory exploration into the landscape of Natural Language Processing. This document analyzes how NLP is portrayed in popular culture versus its actual industrial applications, establishing a baseline understanding of AI communication capabilities.

### 🔹 Module 02: Text Processing and Cleaning
* **Files:**
    * `Lab_02_Chloe_Tu_ITAI_2373.ipynb` (Code Implementation)
    * `L02_Journal_Chloe_Tu_ITAI_2373.pdf` (Reflective Journal)
    *  `L02_Chloe_Tu_ITAI2373.pdf` (L02 AI History Detectives PDF)
* **Description:** Focused on the critical "data wrangling" phase of NLP. I utilized Python libraries to construct a cleaning pipeline that ingests raw text, removes HTML tags and special characters using Regular Expressions (Regex), and normalizes text for downstream analysis. The journal documents the challenges faced during the tokenization process.

### 🔹 Module 03: Audio Preprocessing (Project EchoBlade)
* **Files:**
    * `A03_Chloe_Tu_ITAI_2373.pdf` (Technical Proposal)
    * `L03_Chloe_Tu_ITAI2373_GameDesign.pdf` (L03 AI Game Master PDF Game World Design)
    * `L03_Chloe_Tu_ITAI2373_GameDesign.docx` (L03 AI Game Master Design Doc Source)
* **Description:** A creative proposal for "EchoBlade," a specialized voice recognition system designed for the MMORPG *Legends of the Shattered Realms*.
    * **Challenge:** Solving the "Cocktail Party Problem" in high-noise, reverb-heavy virtual environments.
    * **Solution:** Proposed a Seq2Seq model architecture capable of processing invented fantasy languages and utilizing dereverb algorithms to isolate player commands from background game noise.

### 🔹 Module 04: Introduction to Text Representation
* **Files:**
    * `L04__Chloe_Tu_ITAI_2373.ipynb` (Code Implementation)
    * `L04_Journal_Chloe_Tu_ITAI_2373.pdf` (Reflective Journal)
    * `L04_Chloe_Tu_ITAI_2373.pdf` (L04 Exlore Generative AI for Visualizing Rendering History PDF)
* **Description:** Explored the transformation of unstructured text into numerical vectors that machine learning algorithms can process. Implemented techniques such as **Bag-of-Words (BoW)** and **TF-IDF** (Term Frequency-Inverse Document Frequency) to quantify word importance within a corpus.

### 🔹 Module 05: Part of Speech (POS) Tagging
* **Files:**
    * `L05_Tu_Chloe_ITAI2373.ipynb` (Code Implementation)
    * `L05_Chloe_Tu_ITAI_2373.pdf` (Explore Generative AI for Visualizing Rendering History PDF)
* **Description:** Utilized NLTK to perform automated grammatical tagging. The project involved building a tagger to identify nouns, verbs, adjectives, and other parts of speech, which is a fundamental step for syntactic analysis and named entity recognition.

### 🔹 Module 06: Mapping the Neural Network Brain
* **Files:**
    * `A06_AV_Chloe_Tu__ITAI_2373.pdf` (Audio/Video Walkthrough)
    * `A06_KG_Chloe_Tu__ITAI_2373.pdf` (Knowledge Graph)
    * `A06_RF_Chloe_Tu_ITAI 2373.pdf` (Reflection Report)
* **Description:** A conceptual visualization project that maps the biological functions of the human brain to the architectural components of Artificial Neural Networks (ANNs).
    * **Key Insight:** Mapped *Dendrites* to *Input Layers*, *Synapses* to *Weights*, and *Axons* to *Outputs*. The reflection report discusses the limitations of biological analogies when explaining supervised learning algorithms like Backpropagation.

### 🔹 Module 07: Sentiment and Emotion Analysis
* **Files:**
    * `L07_Chloe_Tu_ITAI2373.ipynb` (Code Implementation)
    * `A07_Chloe_Tu_ITAI_2373.pdf` (Neural Network Architecture Presentation)
    * `L07_Chloe_Tu ITAI_2373.pdf` (L07 Neural Networks Playgrounds PDF)
* **Description:** Designed and visualized a complete Neural Network architecture for an Ad-Click Prediction Model.
    * **Architecture:** Input Layer (Time on Site, Device Type) → Hidden Layers (ReLU Activation) → Output Layer (Sigmoid Function).
    * **Mechanism:** Detailed the mathematical process of Forward Propagation and how Gradient Descent is applied during Backpropagation to minimize the Loss Function.

### 🔹 Module 08: Generative Adversarial Networks (Fact vs. Fiction)
* **Files:**
    * `A08_Chloe_Tu_ITAI_2373.pdf` (Story Analysis Report)
    * `L08_Chloe_Tu_ITAI_2373.pdf` (Lab Report)
* **Description:** A "Turing Test" style experiment designed to simulate the **Discriminator** component of a GAN. I analyzed stories generated by LLMs (Gemini, ChatGPT, Claude) against human-written events to identify patterns of authenticity.
    * **Findings:** "Real" training data relies on specific sensory details and imperfection, while "Generated" fakes often adhere to cliché narrative arcs and perfect resolution.

### 🔹 Module 09: Computer Vision & Image Generation
* **File:** `L09_Chloe_Tu_ITAI_2373.pdf`
* **Description:** An exploration of Multimodal AI, specifically examining platforms that bridge Natural Language Processing prompts with Computer Vision to generate images. This module investigates how text embeddings are translated into visual outputs.

### 🔹 Module 10: Advanced NLP Concepts
* **File:** `L10_Chloe_Tu_ITAI2373.pdf`
* **Description:** A lab report covering specialized advanced techniques in NLP, likely focusing on transformer architectures or specific applications of deep learning in language tasks.

### 🔹 Module 11: AI Digital Assistants
* **Files:**
    * `A11_Chloe_Tu_ITAI_2373.pdf` (Film Analysis)
    * `L11_Chloe_Tu_ITAI_2373.pdf` (Lab Report)
* **Description:** A comparative analysis of the fictional AI "Samantha" from the movie *Her* (2013) versus modern Conversational AI agents. The report evaluates current technological limitations regarding consciousness and emotional reciprocity, while raising ethical concerns about data privacy and user dependency.

### 🔹 Module 12: Predictive Modeling
* **File:** `A12_Chloe_Tu_ITAI2373.pdf`
* **Description:** A narrative project titled **"The Algorithmic Alibi."**
    * **Concept:** Explored the societal impact of predictive policing algorithms.
    * **Technical Focus:** Demonstrated the workflow of predictive modeling (Data Collection → Preprocessing → Training → Evaluation) and highlighted the dangers of "Automation Bias" where humans over-rely on algorithmic probability scores.

### 🔹 Module 13: Robotic Design & Ethical Analysis
* **File:** `A13_Chloe_Tu_ITAI_2373.pdf`
* **Description:** A comprehensive design proposal for **"The Maestro,"** an autonomous entertainment robot for the hospitality industry.
    * **Framework:** Applied the "Perception-Cognition-Action" loop.
    * **Ethics:** Developed strict mitigation strategies for privacy (local-only processing) and safety (collision avoidance sensors) to adhere to core AI ethical principles.

---
