---
name: project-revisao-speech
description: Revisão bibliográfica sistemática PRISMA em Speech Analytics — alunos de IC, suporte à Fase 2, agente em RevisaoSpeech/IA.md
metadata:
  type: project
---

Revisão bibliográfica sistemática sobre Speech Analytics e comunicação clínica, conduzida pelos alunos de IC em paralelo à coleta de dados da Fase 2 do mestrado.

**Por:** Alunos de IC (usuários primários do agente) + Rafael Baena (orientador/revisor).

**Por que:** Produzir um paper de revisão PRISMA autônomo para futura submissão E fundamentar o estado da arte e a lacuna científica do paper principal da Fase 2.

**How to apply:** O agente em `IA.md` guia os alunos passo a passo nas etapas PRISMA. O corpus de partida é o `contexto/BaseCitacoes.md`. O PDF do artigo MCP é apenas template metodológico PRISMA — o tema desta revisão é Speech Analytics.

---

## Estrutura de Pastas

```
RevisaoSpeech/
├── IA.md                          ← agente de IA especializado para esta revisão
├── MEMORIA.md                     ← este arquivo
└── contexto/
    ├── BaseCitacoes.md            ← corpus principal de referências (Grupos A–D + ética)
    └── uma-revisao-sistematica-sobre-a-aplicacao-do-model-context-protocol-mcp-em-ambientes-de-integracao-de-sistemas.pdf
                                   ← modelo estrutural PRISMA (tema MCP, estrutura reutilizável)
```

---

## Conexão com a Fase 2

Esta revisão é subsidiária ao projeto principal da Fase 2 (mestrado em Ciência de Dados em Saúde, USF). O paper principal investiga:

> A anamnese clínica como fonte estruturável de dados comunicacionais e comportamentais, operacionalizada por meio de Speech Analytics.

A revisão sistemática deve estabelecer o estado da arte e confirmar a lacuna que justifica a Fase 2.

---

## Lacuna Central que a Revisão Deve Estabelecer

> Poucos estudos operacionalizam interações clínicas como **variáveis mensuráveis derivadas da fala** — especialmente marcadores comunicacionais e comportamentais (dúvida, dor, barreira, baixa autoeficácia, clareza, engajamento, silêncio). Esta lacuna motiva o paper da Fase 2.

---

## Corpus Principal — BaseCitacoes.md

| Grupo | Tema | Autores-chave |
|-------|------|---------------|
| A | NLP clínico, NER biomédico, extração de sintomas | Bazoge 2023, Navarro 2023, Watabe 2025, Sezgin 2023, Koleck 2019, Wang 2018 |
| B | Documentação automatizada, SOAP, digital scribes, ASR | Krishna 2021, Klusty 2025, Abbasian 2024, Aleksić 2017, Tran 2023, Schloss 2020, van Buchem 2021 |
| C | Comunicação médico-paciente, literacia, adesão | Shao 2025, Muscat 2020, Kelley 2014, Rucinski 2022, McCabe 2018, Alkhamees 2023 |
| D | Biomarcadores vocais, análise multimodal | Fagherazzi 2021, Albert 2024, Imel 2022 |
| E (ética) | CNS 466/2012, LGPD, Lei 14.874/2024, OECD, WHO/OMS, Floridi, COPE | — |

---

## Perguntas de Pesquisa (RQs)

- **RQ1**: Quais abordagens de Speech Analytics têm sido aplicadas à comunicação clínica nos últimos cinco anos?
- **RQ2**: Quais métodos de NLP e ASR são utilizados para transcrição e análise automatizada de consultas clínicas?
- **RQ3**: Quais marcadores comunicacionais e comportamentais foram identificados ou propostos na interação profissional-paciente?
- **RQ4**: Quais são os desafios técnicos, éticos e metodológicos reportados na literatura para a análise automatizada da comunicação clínica?

---

## Estado do Fluxo PRISMA

| Etapa | n | Status |
|-------|---|--------|
| Registros identificados (bases eletrônicas) | — | Em construção |
| Registros de fontes adicionais (BaseCitacoes.md) | — | Em construção |
| Após remoção de duplicatas | — | — |
| Triagem por título/resumo | — | — |
| Excluídos na triagem | — | — |
| Leitura completa | — | — |
| Excluídos após leitura completa | — | — |
| Incluídos na síntese qualitativa | — | — |
| Incluídos na síntese quantitativa | — | — |

Atualizar esta tabela a cada rodada de busca.

---

## Checklist de Qualidade Metodológica

**Dybå & Dingsøyr (Q1–Q5)**, pontuação {0, 0.5, 1}:

| Item | Pergunta |
|------|----------|
| Q1 | A questão de pesquisa está claramente definida? |
| Q2 | O desenho do estudo é adequado para responder à questão? |
| Q3 | Os dados foram coletados de forma sistemática? |
| Q4 | Os resultados foram analisados de forma rigorosa? |
| Q5 | As conclusões estão sustentadas pelos dados apresentados? |

- Score < 2.5 → síntese qualitativa apenas
- Score ≥ 2.5 → elegível para síntese quantitativa

---

## Decisões e Histórico

| Data | Decisão | Por quê |
|------|---------|---------|
| 2026-05-21 | IA.md criado para guiar alunos de IC na revisão PRISMA de Speech Analytics | Alunos conduzem a revisão em paralelo à coleta de dados da Fase 2 |
| 2026-05-21 | PDF do artigo MCP usado apenas como template PRISMA estrutural | O tema da revisão é Speech Analytics, não MCP |
