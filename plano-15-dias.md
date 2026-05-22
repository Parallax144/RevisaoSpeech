# Plano de Trabalho — 15 Dias
## Revisão Sistemática em Speech Analytics e Comunicação Clínica

**Período:** 22/05/2026 — 05/06/2026  
**Equipe:**
- **Rafael** — orientador, aprovações metodológicas, resolução de discordâncias
- **IC-1** — aluno de IC, revisor primário
- **IC-2** — aluno de IC, revisor secundário (kappa)

---

## Semana 1 — Protocolo e Buscas (22–28/mai)

### 22–23/mai — Preparação

| Responsável | Tarefa |
|-------------|--------|
| Rafael | Revisar e aprovar RQs, critérios IC/EC e strings de busca definidos no `IA.md` |
| Rafael | Registrar protocolo em documento interno ou OSF |
| IC-1 | Instalar Zotero + plugin Better BibTeX; criar pasta compartilhada do projeto |
| IC-2 | Instalar Zotero; criar cadastro nas bases que exigem registro (IEEE, Scopus, PubMed) |

### 24/mai — Execução das Buscas (bloco 1)

| Responsável | Tarefa |
|-------------|--------|
| IC-1 | Executar busca no **IEEE Xplore** e **ACM Digital Library**; exportar resultados para Zotero |
| IC-2 | Executar busca no **PubMed/MEDLINE** e **Web of Science**; exportar resultados para Zotero |

### 25–26/mai — Execução das Buscas (bloco 2)

| Responsável | Tarefa |
|-------------|--------|
| IC-1 | Executar busca no **Scopus** e **arXiv**; exportar para Zotero |
| IC-2 | Executar busca no **Google Scholar** (literatura cinzenta); adicionar artigos da `contexto/BaseCitacoes.md` como fonte adicional |
| Rafael | Revisar strings exportadas; validar se os resultados fazem sentido temático |

### 27–28/mai — Consolidação

| Responsável | Tarefa |
|-------------|--------|
| IC-1 | Mesclar bibliotecas no Zotero; remover duplicatas; corrigir metadados incompletos |
| IC-2 | Revisar registros importados; corrigir metadados incompletos |
| Rafael | Confirmar total de registros identificados; preencher os primeiros `[n=X]` do fluxo PRISMA no `MEMORIA.md` |

### ✅ Entregável — Semana 1
- Biblioteca Zotero unificada, sem duplicatas
- Total de registros identificados registrado no `MEMORIA.md`
- Primeiros campos do fluxo PRISMA preenchidos

---

## Semana 2 — Triagem e Avaliação (29/mai–04/jun)

### 29–30/mai — Triagem por Título e Resumo

| Responsável | Tarefa |
|-------------|--------|
| IC-1 | Triar **independentemente** título e resumo — primeira metade dos registros; aplicar IC/EC |
| IC-2 | Triar **independentemente** título e resumo — mesma primeira metade (para cálculo do κ) |
| Rafael | Disponível para consulta sobre casos duvidosos de critérios |

### 31/mai — Kappa e Segunda Metade

| Responsável | Tarefa |
|-------------|--------|
| Rafael | Calcular coeficiente κ com IC-1 e IC-2; resolver discordâncias; registrar resultado |
| IC-1 | Triar independentemente — segunda metade dos registros |
| IC-2 | Triar independentemente — segunda metade dos registros |

### 01/jun — Leitura Completa

| Responsável | Tarefa |
|-------------|--------|
| IC-1 | Leitura completa dos artigos da sua metade; aplicar IC/EC; registrar motivo de exclusão para cada descarte |
| IC-2 | Leitura completa dos artigos da sua metade; aplicar IC/EC; registrar motivo de exclusão para cada descarte |
| Rafael | Validar lista final pós-triagem; liberar para leitura completa |

### 02–03/jun — Avaliação de Qualidade

| Responsável | Tarefa |
|-------------|--------|
| IC-1 | Avaliar qualidade metodológica (Dybå & Dingsøyr Q1–Q5) dos artigos incluídos da sua metade |
| IC-2 | Avaliar qualidade metodológica (Dybå & Dingsøyr Q1–Q5) dos artigos incluídos da sua metade |
| Rafael | Revisar casos limítrofes; decidir inclusões duvidosas |

### 04/jun — Fechamento da Triagem

| Responsável | Tarefa |
|-------------|--------|
| IC-1 | Consolidar tabela de exclusões com código e justificativa |
| IC-2 | Consolidar tabela de scores de qualidade |
| Rafael | Revisar e aprovar o fluxo PRISMA completo; atualizar todos os `[n=X]` no `MEMORIA.md` e no `resumo.tex` |

### ✅ Entregável — Semana 2
- Lista final de artigos incluídos com scores de qualidade
- Tabela de exclusões com justificativas (código E1–E4)
- Fluxo PRISMA com todos os `[n=X]` preenchidos
- `resumo.tex` atualizado com os números reais

---

## Dia 15 — Extração e Planejamento da Síntese (05/jun)

| Responsável | Tarefa |
|-------------|--------|
| Rafael | Reunião de alinhamento: revisar fluxo PRISMA, validar scores, definir divisão da extração |
| IC-1 | Iniciar extração de dados no template do `IA.md` — Grupos A (NLP clínico) e B (documentação automatizada) |
| IC-2 | Iniciar extração de dados no template do `IA.md` — Grupos C (comunicação clínica) e D (biomarcadores vocais) |

### ✅ Entregável — Dia 15
- Fluxo PRISMA finalizado e commitado no repositório
- Extração iniciada nos quatro grupos temáticos
- Pauta definida para a semana 3 (síntese e redação)

---

## Ferramentas Necessárias

| Ferramenta | Para quê | Responsável pela configuração |
|------------|----------|-------------------------------|
| Zotero + Better BibTeX | Gerenciar referências e exportar `.bib` | IC-1 (instala e compartilha) |
| Planilha compartilhada (Google Sheets) | Triagem IC/EC, scores de qualidade, extração | Rafael cria o template |
| Claude + `IA.md` | Apoio metodológico em cada etapa PRISMA | Todos |
| GitHub (`revisaospeech`) | Versionar arquivos de trabalho | Rafael commita marcos principais |

---

## Critérios de Inclusão e Exclusão (referência rápida)

| Inclusão (IC) | Exclusão (EC) |
|---|---|
| IC1: Aplica Speech Analytics, NLP ou ASR a contexto clínico | EC1: Publicações anteriores a 2018 |
| IC2: Texto completo em inglês, português ou espanhol | EC2: Resumos estendidos, tutoriais sem dados |
| IC3: Analisa comunicação profissional-paciente ou extração de informação de consultas | EC3: Foco exclusivo em diagnóstico por voz de patologias físicas sem análise comunicacional |
| IC4: Descreve métodos, resultados ou marcadores aplicáveis à interação clínica | EC4: Estudos sobre populações não clínicas sem transferibilidade metodológica explícita |

---

## Checklist de Qualidade — Dybå & Dingsøyr

| Item | Pergunta | Pontuação |
|------|----------|-----------|
| Q1 | A questão de pesquisa está claramente definida? | 0 / 0,5 / 1 |
| Q2 | O desenho do estudo é adequado para responder à questão? | 0 / 0,5 / 1 |
| Q3 | Os dados foram coletados de forma sistemática? | 0 / 0,5 / 1 |
| Q4 | Os resultados foram analisados de forma rigorosa? | 0 / 0,5 / 1 |
| Q5 | As conclusões estão sustentadas pelos dados apresentados? | 0 / 0,5 / 1 |

> Score < 2,5 → síntese qualitativa apenas  
> Score ≥ 2,5 → elegível para síntese quantitativa

---

## Fluxo PRISMA — Registro Incremental

| Etapa | n | Responsável | Prazo |
|-------|---|-------------|-------|
| Registros identificados (bases eletrônicas) | [n=X] | IC-1 + IC-2 | 26/mai |
| Registros de fontes adicionais (BaseCitacoes.md) | [n=X] | IC-2 | 26/mai |
| Após remoção de duplicatas | [n=X] | IC-1 | 28/mai |
| Excluídos na triagem título/resumo | [n=X] | IC-1 + IC-2 | 31/mai |
| Artigos para leitura completa | [n=X] | IC-1 + IC-2 | 31/mai |
| Excluídos após leitura completa | [n=X] | IC-1 + IC-2 | 04/jun |
| Incluídos na síntese qualitativa | [n=X] | Rafael | 04/jun |
| Incluídos na síntese quantitativa | [n=X] | Rafael | 04/jun |
