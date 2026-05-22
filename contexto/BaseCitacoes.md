Relatório Técnico Expandido: Protocolo de Speech Analytics e IA para Reabilitação Ortopédica no SUS

1. Introdução e Contextualização do Protocolo

Este relatório apresenta a fundamentação científica e o arcabouço normativo do "Protocolo metodológico baseado em análise da fala para monitoramento da reabilitação ortopédica no SUS", projeto sob responsabilidade do pesquisador Vicente Idalberto Becerra Sablon e da Universidade São Francisco (USF). A iniciativa propõe uma solução disruptiva para o Sistema Único de Saúde (SUS), visando a extração de indicadores de comunicação terapêutica e adesão ao tratamento por meio de inteligência artificial.

Justificado pelo impacto das condições musculoesqueléticas — que afetam cerca de 1,71 bilhão de pessoas globalmente e são a maior causa de incapacidade funcional —, o protocolo atua sobre a lacuna de monitoramento sistemático no serviço público. O fluxo tecnológico desenhado integra as etapas de:

1. Reconhecimento Automático de Fala (ASR): Conversão de áudio clínico em texto.
2. Diarização de Locutores: Segregação de turnos de fala entre profissional e paciente.
3. Processamento Semântico (LLMs): Interpretação contextual e extração de entidades biomédicas.
4. Indexação Semântica: Organização dos vetores de informação para recuperação ágil.
5. Análise via RAG (Geração Aumentada por Recuperação): Ancoragem das respostas do modelo em fatos clínicos reais (groundedness), mitigando alucinações algorítmicas.


--------------------------------------------------------------------------------


2. Compilação da Base Científica (IA, NLP e Comunicação em Saúde)

A base de evidências abaixo reúne a totalidade dos artigos que fundamentam a arquitetura Sablon, organizados por afinidade temática e contribuição específica.

Grupo A: NLP, Extração de Sintomas e Entidades Biomédicas

Título: Applying Natural Language Processing to Textual Data From Clinical Data Warehouses: Systematic Review
Autores: Adrien Bazoge, Emmanuel Morin, Béatrice Daille, Pierre-Antoine Gourraud
Ano: 2023
Periódico: JMIR Medical Informatics
Link: doi: 10.2196/42477
Resumo: Revisão sistemática sobre o uso de NLP em armazéns de dados clínicos (CDWs), evidenciando a migração de métodos simbólicos para modelos de deep learning e transformers.
Contribuição: Justifica o reaproveitamento de dados secundários e o uso de transformers para fenotipagem e gestão de sintomas no protocolo proposto.


--------------------------------------------------------------------------------


Título: Clinical named entity recognition and relation extraction using natural language processing of medical free text: A systematic review
Autores: David Fraile Navarro, et al.
Ano: 2023
Periódico: International Journal of Medical Informatics
Link: https://doi.org/10.1016/j.ijmedinf.2023.105122
Resumo: Valida que modelos como BERT lideram a extração de "problemas" e "tratamentos", mas aponta a escassez de implementações no mundo real.
Contribuição: Suporta a Etapa 2 do protocolo (NER Biomédico) e a necessidade de levar a tecnologia do laboratório para o ambiente hospitalar do SUS.


--------------------------------------------------------------------------------


Título: A patient-centered approach to developing and validating a natural language processing model for extracting patient-reported symptoms
Autores: Satoshi Watabe, et al.
Ano: 2025
Periódico: Scientific Reports
Link: https://doi.org/10.1038/s41598-025-12845-3
Resumo: Desenvolveu um modelo BERT-CRF para extração de sintomas em linguagem coloquial com F1-score > 0.8.
Contribuição: Demonstra a necessidade de fine-tuning com dados narrativos autênticos para capturar gírias e sutilezas da fala do paciente ortopédico.


--------------------------------------------------------------------------------


Título: Extracting Medical Information From Free-Text and Unstructured Patient-Generated Health Data Using Natural Language Processing Methods: Feasibility Study With Real-world Data
Autores: Emre Sezgin, et al.
Ano: 2023
Periódico: JMIR Formative Research
Link: doi:10.2196/43014
Resumo: Utiliza NER e ontologias (SNOMED CT) em abordagem "zero-shot" para identificar sintomas em dados gerados por pacientes.
Contribuição: Valida a viabilidade de modelos pré-treinados para traduzir linguagem leiga em métricas clínicas, essencial para a telemedicina no SUS.


--------------------------------------------------------------------------------


Título: Natural language processing of symptoms documented in free-text narratives of electronic health records: a systematic review
Autores: Theresa A. Koleck, et al.
Ano: 2019
Periódico: Journal of the American Medical Informatics Association (JAMIA)
Link: 10.1093/jamia/ocy173
Resumo: Sintetiza o sucesso de algoritmos de classificação na extração de sintomas subjetivos (dor, humor) documentados em texto livre.
Contribuição: Alinha-se à extração de "patient reported symptoms" durante a anamnese reabilitadora.


--------------------------------------------------------------------------------


Título: Clinical Information Extraction Applications: A Literature Review
Autores: Yanshan Wang, et al.
Ano: 2018
Periódico: Journal of Biomedical Informatics
Link: https://doi.org/10.1016/j.jbi.2017.11.011
Resumo: Revisão histórica de 263 estudos evidenciando a adesão médica a sistemas de regras linguísticas (cTAKES, MedLEE).
Contribuição: Fornece a ponte entre a automação clássica e o Machine Learning exigido pelo volume de dados do SUS.


--------------------------------------------------------------------------------


Grupo B: Documentação Clínica Automatizada, Notas SOAP e Validação Técnica

Título: Generating SOAP Notes from Doctor-Patient Conversations Using Modular Summarization Techniques
Autores: Kundan Krishna, et al.
Ano: 2021
Periódico: Carnegie Mellon University / Conference Proceedings
Link: https://doi.org/10.48550/arXiv.2005.01795
Resumo: Introduz o modelo CLUSTER2SENT para gerar notas estruturadas (SOAP) a partir de conversas densas.
Contribuição: Fundamenta a estruturação das saídas analíticas do protocolo, permitindo ao fisioterapeuta localizar evidências verbais rapidamente.


--------------------------------------------------------------------------------


Título: Toward Automated Clinical Transcriptions
Autores: Mitchell A. Klusty, et al.
Ano: 2025
Periódico: University of Kentucky
Link: https://pmc.ncbi.nlm.nih.gov/articles/PMC12150720/
Resumo: Sistema baseado em OpenAI Whisper e PyAnnote operando em servidores fechados para garantir privacidade.
Contribuição: Resolve o desafio da diarização e segurança de dados (on-premise), requisito ético para implantação hospitalar.


--------------------------------------------------------------------------------


Título: Foundation metrics for evaluating effectiveness of healthcare conversations powered by generative AI
Autores: Mahyar Abbasian, et al.
Ano: 2024
Periódico: npj Digital Medicine
Link: https://doi.org/10.1038/s41746-024-01074-z
Resumo: Propõe métricas de segurança, validade factual (groundedness) e empatia para IAs generativas na saúde.
Contribuição: Pauta a introdução obrigatória de RAG no fluxo do Sablon para garantir que os indicadores sejam baseados exclusivamente em fatos extraídos da consulta.


--------------------------------------------------------------------------------


Título: Data summarization method for chronic disease tracking
Autores: Dejan Aleksić, et al.
Ano: 2017
Periódico: Journal of Biomedical Informatics
Link: http://dx.doi.org/10.1016/j.jbi.2017.04.012
Resumo: Modelo integrado para resumir EHR visando detectar pacientes que precisam de atenção especializada.
Contribuição: Valida o uso de dashboards e resumos fáceis de ler para reduzir a carga cognitiva do profissional no SUS.


--------------------------------------------------------------------------------


Título: Automatic speech recognition performance for digital scribes: a performance comparison between general-purpose and specialized models
Autores: Brian D. Tran, et al.
Ano: 2023
Periódico: AMIA / University of California
Link: https://pmc.ncbi.nlm.nih.gov/articles/PMC10148344/
Resumo: Demonstra que falhas em pronomes curtos ("eu", "você") em modelos de ASR são mais críticas do que em termos médicos complexos.
Contribuição: Alerta para a necessidade de precisão na casualidade da fala para garantir a validade dos indicadores de adesão.


--------------------------------------------------------------------------------


Título: Towards an Automated SOAP Note: Classifying Utterances from Medical Conversations
Autores: Benjamin Schloss, Sandeep Konam
Ano: 2020
Periódico: Proceedings of Machine Learning Research
Link: https://doi.org/10.48550/arXiv.2007.08749
Resumo: Usa redes Bi-LSTMs hierárquicas para classificar frases da consulta nas seções SOAP com alta precisão.
Contribuição: Define estratégias modulares para tratar a "poluição" de dados em transcrições automáticas ruidosas.


--------------------------------------------------------------------------------


Título: The digital scribe in clinical practice: a scoping review and research agenda
Autores: Marieke M. van Buchem, et al.
Ano: 2021
Periódico: npj Digital Medicine
Link: https://doi.org/10.1038/s41746-021-00432-5
Resumo: Aponta a falta de estudos prospectivos de usabilidade e utilidade clínica real para escribas digitais.
Contribuição: Reforça a importância do desenho prospectivo do protocolo para transpor a prova de conceito para a validação clínica real.


--------------------------------------------------------------------------------


Grupo C: Comunicação Médico-Paciente, Literacia e Adesão

Título: Development of a measurement of doctor-patient communication quality scale
Autores: Jiayi Shao, et al.
Ano: 2025
Periódico: Frontiers in Public Health
Link: doi: 10.3389/fpubh.2025.1606403
Resumo: Escala DPCQ de 14 itens focada em suporte emocional e educação em saúde.
Contribuição: Provê as categorias semânticas (interação emocional vs. orientação comportamental) para as métricas automáticas do protocolo.


--------------------------------------------------------------------------------


Título: Health Literacy and Shared Decision-making
Autores: Danielle M. Muscat, et al.
Ano: 2020
Periódico: Journal of General Internal Medicine
Link: DOI: 10.1007/s11606-020-05912-0
Resumo: Indica que a tomada de decisão compartilhada exige construir habilidades no paciente via instrução verbal eficaz.
Contribuição: Valida que o monitoramento da fala no SUS deve capturar o sucesso da literacia em saúde, substituindo cartilhas passivas por escuta ativa.


--------------------------------------------------------------------------------


Título: The Influence of the Patient-Clinician Relationship on Healthcare Outcomes: A Systematic Review and Meta-Analysis
Autores: John M. Kelley, et al.
Ano: 2014
Periódico: PLoS ONE
Link: 10.1371/journal.pone.0094207
Resumo: Meta-análise que prova o impacto significativo da comunicação emocional e cognitiva nos desfechos objetivos de saúde.
Contribuição: Referência fundamental para justificar o investimento tecnológico em métricas de qualidade do relacionamento clínico.


--------------------------------------------------------------------------------


Título: Patient and Healthcare Team Adherence in Orthopaedics: A Systematic Review
Autores: Kylee Rucinski, et al.
Ano: 2022
Periódico: Journal of Patient Care
Link: DOI: 10.35248/2573-4598.22.8.203
Resumo: Demonstra que métricas atuais falham ao ignorar as barreiras impostas pela equipe e pelo sistema de saúde.
Contribuição: Sustenta a criação de "dados auditáveis" para mapear falhas bilaterais (equipe/paciente) na reabilitação ortopédica.


--------------------------------------------------------------------------------


Título: Miscommunication in Doctor–Patient Communication
Autores: Rose McCabe, Patrick G. T. Healey
Ano: 2018
Periódico: Topics in Cognitive Science
Link: DOI: 10.1111/tops.12337
Resumo: Comprova que o uso de "autorreparo" na fala médica prediz uma adesão superior ao tratamento.
Contribuição: Valida a análise de dinâmicas microscópicas da fala (mapeáveis por IA) como preditores de adesão no SUS.


--------------------------------------------------------------------------------


Título: Patient-physician communication in intercultural settings: An integrative review
Autores: Mohammad Alkhamees, Ibrahim Alasqah
Ano: 2023
Periódico: Heliyon
Link: https://doi.org/10.1016/j.heliyon.2023.e22667
Resumo: Mapeia como disparidades linguísticas e estilos autoritários geram inibição em pacientes e decisões clínicas ruins.
Contribuição: Relevante para o contexto diversificado do SUS, identificando barreiras invisíveis aos gestores através do Speech Analytics.


--------------------------------------------------------------------------------


Grupo D: Biomarcadores Vocais e Análise Multimodal

Título: Voice for Health: The Use of Vocal Biomarkers from Research to Clinical Practice
Autores: Guy Fagherazzi, et al.
Ano: 2021
Periódico: Digital Biomarkers
Link: 10.1159/000515346
Resumo: Descreve o pipeline para capturar características linguísticas e acústicas que indicam estados de saúde e emoções.
Contribuição: Fundamenta a etapa de identificação de sinais clínicos diretamente da voz, além da semântica do texto.


--------------------------------------------------------------------------------


Título: A scoping review of AI, speech and natural language processing methods for assessment of clinician-patient communication
Autores: Pierre Albert, et al.
Ano: 2024
Periódico: medRxiv
Link: https://doi.org/10.1101/2024.12.13.24318778
Resumo: Ressalta a carência de estudos em linguagem não verbal, tons de voz e silêncios.
Contribuição: Direciona o protocolo para uma análise multimodal futura, onde pausas são componentes terapêuticos mapeáveis.


--------------------------------------------------------------------------------


Título: Identifying Topics in Patient and Doctor Conversations Using Natural Language Processing Methods
Autores: Zac Imel, et al.
Ano: 2022
Periódico: PCORI Final Research Report
Link: https://doi.org/10.25302/08.2021.me.160234167
Resumo: Mapeia valências emocionais em consultas via redes neurais sequenciais, atingindo concordância similar a juízes humanos.
Contribuição: Pavimenta o uso de NLP para medir a empatia e o atendimento humanizado em larga escala no SUS.


--------------------------------------------------------------------------------


3. Referências Éticas e Regulatórias

A transição da arquitetura metodológica para o ambiente prático do SUS exige conformidade com o arcabouço normativo brasileiro e internacional. O protocolo é regido pelas seguintes diretrizes:

Diretrizes Nacionais e Internacionais

* Resolução CNS nº 466/2012: Norma regulamentadora de pesquisas com seres humanos no Brasil.
* Lei nº 14.874/2024: Estabelece os requisitos rigorosos para a condução de ensaios clínicos e o rito de proteção aos participantes.
* Registro Brasileiro de Ensaios Clínicos (ReBEC): Plataforma obrigatória para registro de protocolos clínicos nacionais.
* Committee on Publication Ethics (COPE): Padrões de integridade em redação e publicação técnico-científica.
* OECD (2021) & WHO (2024): Princípios de ética em IA na saúde e transparência em registros internacionais de ensaios clínicos (ICTRP).
* L. Floridi (2018): Base filosófica para a governança ética de ciência de dados e algoritmos.

Lições de Governança: Do Modelo Experimental à Realidade SUS

Em conformidade com o Parecer CEP nº 8.367.023, a implementação do protocolo identificou pontos críticos de governança. Para a transição da atual fase (dados secundários SIA/SIH e sintéticos) para a coleta de dados primários (gravação de consultas reais), o pesquisador deve observar:

1. Estruturação de Projeto vs. Manuscrito: Conforme apontado pelo comitê, é imperativo submeter um Projeto de Pesquisa estruturado e não apenas um manuscrito científico, sob pena de retirada do rito avaliativo.
2. Harmonização Metodológica: Devem ser sanadas discrepâncias entre o cadastro na Plataforma Brasil e o corpo do texto (ex: amostras citadas de 390 vs 3 participantes), assegurando a fidedignidade dos dados.
3. Compulsoriedade do TCLE: Dada a natureza da coleta de voz (biometria), a dispensa do Termo de Consentimento Livre e Esclarecido não é aplicável para a gravação de interações, exigindo nova submissão ética para qualquer validação clínica real com seres humanos.


--------------------------------------------------------------------------------


4. Riscos, Benefícios e Salvaguardas Metodológicas

A viabilidade do protocolo é sustentada por uma análise equilibrada entre inovação e proteção:

Dimensão	Descrição
Riscos Indiretos	Interpretações inadequadas por LLMs; limitações de dados sintéticos que podem não capturar a complexidade clínica real; vieses algorítmicos em subpopulações.
Benefícios Indiretos	Inovação tecnológica no SUS; melhoria na gestão da reabilitação ortopédica; criação de indicadores auditáveis de adesão e humanização.
Salvaguardas	Uso restrito ao âmbito conceitual/metodológico nesta fase; proibição de uso para decisão clínica imediata; necessidade de aprovação ética prévia para coleta de voz.


--------------------------------------------------------------------------------


5. Considerações Finais e Próximos Passos

O protocolo Sablon representa o estado da arte na integração entre Speech Analytics e a gestão pública de saúde. Ao converter interações verbais tradicionalmente efêmeras em dados estruturados via pipelines de NLP validados (como BERT-CRF e RAG), o projeto resolve o desafio histórico do monitoramento da adesão terapêutica na ortopedia.

A transparência algorítmica e o rigor ético-administrativo — evidenciados pela necessidade de projetos estruturados conforme a Lei nº 14.874/2024 — são os pilares para que esta inovação ganhe escala no SUS. O protocolo está apto a evoluir para validações clínicas prospectivas, consolidando a inteligência de dados como um vetor de eficiência e humanização no cuidado especializado brasileiro.
