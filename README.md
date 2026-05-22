# Revisão Bibliográfica Sistemática em Speech Analytics

Repositório de apoio à revisão sistemática da literatura sobre **Speech Analytics e comunicação clínica**, conduzida pelos alunos de Iniciação Científica (IC) do projeto de mestrado em Ciência de Dados em Saúde — Universidade São Francisco (USF).

---

## Objetivo

Produzir uma revisão sistemática seguindo o modelo **PRISMA 2020** sobre o uso de Speech Analytics, NLP e análise automatizada da comunicação profissional-paciente. O trabalho tem dois propósitos articulados:

1. **Paper autônomo** para futura submissão a periódico científico.
2. **Fundamentação da Fase 2 do mestrado**: estabelecer o estado da arte e a lacuna científica que justifica o estudo sobre a anamnese clínica como fonte estruturável de dados comunicacionais e comportamentais.

---

## Estrutura do Repositório

```
revisaospeech/
├── README.md                  ← este arquivo
├── IA.md                      ← agente de IA — leia antes de começar
├── MEMORIA.md                 ← contexto e estado atual do projeto
└── contexto/
    ├── BaseCitacoes.md        ← corpus inicial de referências (Grupos A–D)
    └── *.pdf                  ← modelo estrutural de revisão PRISMA
```

---

## Como Usar o Agente de IA

O arquivo `IA.md` é o **guia central do agente**. Ele deve ser carregado como contexto do Claude (ou outro LLM) no início de cada sessão de trabalho.

### Passo 1 — Abrir o agente

No Claude Code (terminal) ou no Claude.ai, carregue o `IA.md` como contexto:

```
Leia o arquivo IA.md e assuma o papel descrito nele.
Em seguida, leia também o MEMORIA.md e o contexto/BaseCitacoes.md.
```

### Passo 2 — Informar a tarefa

Depois de carregar o contexto, descreva o que você precisa fazer. Exemplos:

```
Quero triar os artigos do Grupo A da BaseCitacoes.md
aplicando os critérios de inclusão e exclusão da revisão.
```

```
Extraia os dados dos artigos do Grupo B no template de extração.
```

```
Escreva um parágrafo do estado da arte sobre digital scribes
com base nos estudos extraídos.
```

```
Quais artigos da BaseCitacoes.md abordam marcadores
comunicacionais ou comportamentais na interação clínica?
```

### Passo 3 — Seguir o fluxo PRISMA

O agente guia você pelas etapas em ordem:

| Etapa | O que fazer |
|-------|-------------|
| 1 | Definir protocolo (RQs, período, bases, strings de busca, IC/EC) |
| 2 | Executar buscas nas bases (IEEE, PubMed, Scopus, arXiv…) |
| 3 | Importar resultados e remover duplicatas |
| 4a | Triagem por título e resumo (dois revisores + kappa) |
| 4b | Leitura completa com aplicação dos IC/EC |
| 5 | Avaliação de qualidade (Dybå & Dingsøyr Q1–Q5) |
| 6 | Extração de dados no template padronizado |
| 7 | Síntese qualitativa e quantitativa por eixo temático e RQ |
| 8 | Redação das seções com rastreabilidade frase a frase |

---

## Regras de Uso do Agente

> O agente **não inventa referências, dados ou conclusões**.  
> Se uma afirmação não puder ser sustentada pelo material fornecido, ele sinaliza a lacuna e pede mais evidência.

- Forneça sempre o material de referência (artigo, resumo, trecho) junto com a tarefa.
- Não peça ao agente para "completar" seções sem fonte — ele irá recusar ou sinalizar.
- Revise toda redação gerada antes de incorporar ao manuscrito.
- Dúvidas metodológicas sobre o PRISMA devem ser levadas ao orientador.

---

## Corpus Inicial

O arquivo `contexto/BaseCitacoes.md` contém o ponto de partida da revisão, organizado em grupos temáticos:

| Grupo | Tema |
|-------|------|
| A | NLP clínico, extração de entidades biomédicas, sintomas em texto livre |
| B | Documentação automatizada, notas SOAP, digital scribes, ASR clínico |
| C | Comunicação médico-paciente, literacia em saúde, adesão ao tratamento |
| D | Biomarcadores vocais, análise multimodal, Speech Analytics em saúde |

Este corpus deve ser **ampliado** com novas buscas nas bases científicas. Os artigos novos passam pela triagem IC/EC antes de entrar na síntese.

---

## Lacuna Científica que a Revisão Deve Estabelecer

> Poucos estudos operacionalizam interações clínicas como **variáveis mensuráveis derivadas da fala** — especialmente marcadores comunicacionais e comportamentais como dúvida, dor, barreira, baixa autoeficácia, clareza, engajamento e silêncio.

A revisão deve mapear o que já existe e evidenciar essa lacuna, que justifica a pesquisa da Fase 2.

---

## Perguntas de Pesquisa

- **RQ1** — Quais abordagens de Speech Analytics têm sido aplicadas à comunicação clínica nos últimos cinco anos?
- **RQ2** — Quais métodos de NLP e ASR são utilizados para transcrição e análise automatizada de consultas clínicas?
- **RQ3** — Quais marcadores comunicacionais e comportamentais foram identificados ou propostos na interação profissional-paciente?
- **RQ4** — Quais são os desafios técnicos, éticos e metodológicos para a análise automatizada da comunicação clínica?

---

## Contribuindo

1. Faça suas extrações e sínteses em arquivos separados dentro de uma pasta `trabalho/`.
2. Atualize a tabela do fluxo PRISMA no `MEMORIA.md` após cada rodada de busca.
3. Abra um commit por etapa concluída — facilita o rastreamento do progresso.

---

## Orientação

Projeto de Mestrado em Ciência de Dados em Saúde — USF  
Pesquisador responsável: Rafael Baena Neto
