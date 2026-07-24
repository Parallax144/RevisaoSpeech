# Estratégia de Busca e Justificativa de Bases de Dados

Este documento registra o planejamento metodológico de busca de literatura para a scoping review, detalhando o comportamento de busca em cada base de dados selecionada e fornecendo as strings de busca formatadas.

---

## 1. Justificativa das Bases de Dados e Cobertura de Busca

Para assegurar uma cobertura ampla e em conformidade com as diretrizes do PRISMA-ScR e do Joanna Briggs Institute (JBI), a busca bibliográfica eletrônica foi expandida e adaptada às particularidades de cada motor de busca:

### A. PubMed/MEDLINE (Base de Dados Primária)
*   **Abordagem:** Utilização de **todas as 6 estratégias de busca** (Strings 1 a 5 + String Geral Unificada).
*   **Racional:** O PubMed é a nossa principal fonte de dados devido à sua vasta cobertura indexada nas áreas biomédica, clínica e de informática em saúde. Ele permite o processamento de consultas booleanas complexas sem limite restritivo de caracteres.

### B. Cochrane Library (Foco em Ensaios Clínicos e Revisões)
*   **Abordagem:** Utilização estritamente da **String 1**.
*   **Racional:** A Cochrane Library é focada especificamente em ensaios clínicos controlados aleatorizados (CENTRAL) e revisões sistemáticas de intervenções em saúde. A **String 1** (sintomas + prontuário eletrônico + NLP) é a que melhor se alinha com o foco de intervenção clínica desta biblioteca. Strings puramente técnicas (como Eixos 2, 4 e 5) não retornariam dados devido à ausência de desenvolvimento puramente computacional/algoritmos no escopo da base.

### C. Google Acadêmico / Google Scholar (Busca Suplementar de Literatura)
*   **Abordagem:** Utilização das **Strings 1 a 5** (com o filtro de título `allintitle:`), **excluindo a String Geral**.
*   **Racional:** O Google Acadêmico possui um limite estrito de **256 caracteres** em sua caixa de busca, impossibilitando a execução de strings aninhadas excessivamente longas como a String Geral Unificada. Além disso, para a **String 5**, foi aplicado um foco específico direcionado à literatura de revisões sistemáticas existentes para mapeamento do estado da arte técnica.

---

## 2. Relação de Strings por Base de Dados

### 2.1. PubMed/MEDLINE (Padrão Original)

*   **String 1 (Eixo A - PLN, Sintomas e Prontuários):**
    ```text
    ("natural language processing"[Title/Abstract]) AND (symptoms[Title/Abstract] OR "patient-reported symptoms"[Title/Abstract]) AND ("electronic health records"[Title/Abstract] OR "patient-centered"[Title/Abstract])
    ```
*   **String 2 (Eixo A - Extração de Informação Clínica e NER):**
    ```text
    ("clinical information extraction"[Title/Abstract] OR "medical information extraction"[Title/Abstract] OR "named entity recognition"[Title/Abstract]) AND ("medical free text"[Title/Abstract] OR "review"[Title/Abstract] OR "patient-generated health data"[Title/Abstract])
    ```
*   **String 3 (Eixo C - Comunicação Clínico-Paciente e Desfechos):**
    ```text
    ("patient-physician communication"[Title/Abstract] OR "doctor-patient communication"[Title/Abstract] OR "patient-clinician relationship"[Title/Abstract]) AND ("intercultural settings"[Title/Abstract] OR miscommunication[Title/Abstract] OR "healthcare outcomes"[Title/Abstract] OR "shared decision-making"[Title/Abstract] OR "communication quality scale"[Title/Abstract])
    ```
*   **String 4 (Eixo D - Biomarcadores Vocais e Speech Analytics):**
    ```text
    ("vocal biomarkers"[Title/Abstract] OR "speech analytics"[Title/Abstract]) AND ("clinical practice"[Title/Abstract] OR "voice for health"[Title/Abstract] OR "SUS"[Title/Abstract])
    ```
*   **String 5 (Eixo B/D - NLP, Speech e Revisões):**
    ```text
    (("Applying natural language processing"[Title/Abstract]) AND ("Systematic review"[Title/Abstract])) OR (("Identifying Topics"[Title/Abstract]) AND ("Natural Language Processing Methods"[Title/Abstract])) OR (("Automatic speech recognition"[Title/Abstract]) AND ("patient-clinician conversations"[Title/Abstract]))
    ```
*   **String Geral Unificada:**
    ```text
    ("speech analytics" OR "speech analysis" OR "speech recognition" OR "automatic speech recognition" OR ASR OR "digital scribe" OR "clinical transcription" OR "clinical documentation" OR "vocal biomarkers" OR "healthcare conversations" OR "doctor-patient conversations" OR "patient-doctor conversations") AND ("natural language processing" OR NLP OR "large language model" OR LLM OR "information extraction" OR "clinical information extraction" OR "named entity recognition" OR NER OR "relation extraction" OR "text mining" OR "conversation analysis" OR "topic modeling" OR "SOAP note" OR "SOAP notes") AND (healthcare OR clinical OR medicine OR medical OR physician OR clinician OR doctor OR patient OR "electronic health record" OR EHR OR hospital OR outpatient)
    ```

---

### 2.2. Cochrane Library

*   **String 1 (Única aplicada):**
    ```text
    ("natural language processing"):ti,ab,kw AND (symptom* OR "patient-reported symptoms"):ti,ab,kw AND ("electronic health records" OR "patient-centered"):ti,ab,kw
    ```

---

### 2.3. Google Acadêmico (Google Scholar - Filtro de Título)

*   **String 1:**
    ```text
    allintitle: "natural language processing" symptoms ("electronic health records" OR "patient-centered")
    ```
*   **String 2:**
    ```text
    allintitle: ("clinical information extraction" OR "named entity recognition") ("medical free text" OR review)
    ```
*   **String 3:**
    ```text
    allintitle: ("doctor-patient communication" OR "patient-clinician relationship") ("shared decision-making" OR outcomes)
    ```
*   **String 4:**
    ```text
    allintitle: ("vocal biomarkers" OR "speech analytics") ("clinical practice" OR SUS)
    ```
*   **String 5 (Filtro focado em Revisão Sistemática):**
    ```text
    allintitle: "Applying natural language processing" OR "Identifying Topics" OR "Automatic speech recognition"
    ```

---

## 3. Texto Proposto para a Metodologia (Seção 3.3 do main.tex)

Abaixo estão as redações propostas em Português (para a versão de revisão atual do `main.tex`) e em Inglês (para a tradução final), detalhando exatamente os critérios que você especificou:

### Versão em Português
> A base de dados primária selecionada pelos pesquisadores foi o PubMed/MEDLINE, na qual foram aplicadas todas as seis estratégias de busca formuladas (sendo cinco strings especializadas em eixos temáticos específicos e uma string geral unificada). Para as demais bases de dados eletrônicas consultadas (Google Scholar, EBSCO/CINAHL, Web of Science e Cochrane Library), foram executadas apenas as cinco strings especializadas correspondentes aos eixos. Como critérios de busca e filtros eletrônicos gerais, estabeleceu-se o período de publicação entre janeiro de 2014 e 2026, e a seleção de artigos nos idiomas inglês, espanhol e português. Adicionalmente, na base PubMed/MEDLINE, aplicou-se inicialmente o filtro de texto completo gratuito (*free full text*) em decorrência de limitações de acesso institucional a artigos sob paywall.

### Versão em Inglês (Final translation)
> The primary database selected by the researchers was PubMed/MEDLINE, in which all six formulated search strategies were applied (comprising five strings specialized in specific thematic axes and one unified general string). For the other electronic databases consulted (Google Scholar, EBSCO/CINAHL, Web of Science, and Cochrane Library), only the five specialized strings were executed. As general search criteria and electronic filters, the publication period was restricted from January 2014 to 2026, and studies published in English, Spanish, and Portuguese were selected. Additionally, in the PubMed database, the free full-text filter was applied due to initial institutional access limitations to paywalled articles.

