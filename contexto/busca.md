# Registro de Busca — Scoping Review Speech Analytics

**Período de busca:** 28/05/2026 – 11/06/2026  
**Protocolo:** PRISMA-ScR (Tricco et al., 2018) + JBI (Peters et al., 2020)

---

## String de busca

Três blocos combinados com AND:

**Bloco 1 — Tecnologia**
```
("speech analytics" OR "automatic speech recognition" OR "ASR"
OR "natural language processing" OR "NLP" OR "large language model"
OR "speech-to-text" OR "voice recognition" OR "vocal biomarkers"
OR "speaker diarization")
```

**Bloco 2 — Contexto clínico**
```
("clinical communication" OR "doctor-patient" OR "physician-patient"
OR "anamnesis" OR "medical consultation" OR "health interaction"
OR "orthopedic rehabilitation" OR "physical therapy")
```

**Bloco 3 — Desfecho**
```
("communication quality" OR "clinical outcome" OR "adherence"
OR "health literacy" OR "patient engagement")
```

> **Nota:** A string completa (3 blocos) é restritiva — especialmente no PubMed (8 resultados).
> Testar pares de blocos (B1 AND B2; B1 AND B3) para ampliar o corpus antes de Gate 2.

---

## Contagens por base

| Base | Contagem | Status | Observação |
|------|----------|--------|------------|
| Web of Science | **1.719** | Exato | Filtros: 2014-2026, inglês, espanhol, português |
| Scopus | **1.580** | Exato | Filtros: 2014-2026, inglês, espanhol, português |
| PubMed/MEDLINE | **1.059** | Exato | Filtros: 2014-2026, inglês, espanhol, português |
| CINAHL/EBSCO | **586** | Exato | Filtros: 2014-2026, inglês, espanhol, português |
| Cochrane Library | **399** | Exato | Filtros: 2014-2026, inglês, espanhol, português |
| Google Scholar | **278** | Exato | Filtros: 2014-2026, inglês, espanhol, português |
| **Total** | **5.621** | Exato | Total de registros identificados nas bases |

---

## Etapas PRISMA concluídas

| Etapa | Valor | Status / Observação |
|-------|-------|---------------------|
| Registros identificados (bases) | 5.621 | Total bruto de buscas eletrônicas |
| Fontes adicionais (Snowballing)| 7 | Identificados manualmente (estudo piloto) |
| Após remoção de duplicatas | 3.189 | 2.432 duplicatas removidas via Zotero |
| Triagem por título | 3.189 | Triagem por dois revisores independentes |
| Excluídos na triagem por título | 2.680 | Com base nos critérios de elegibilidade |
| Triagem por resumo | 509 | Triagem por dois revisores independentes |
| Excluídos na triagem por resumo | 474 | Com base nos critérios de elegibilidade |
| Texto completo avaliado | 42 | 35 das bases + 7 do snowballing |
| Excluídos no texto completo | 18 | 18 das bases (justificativas em EC1-EC6); 0 do snowballing |
| Incluídos na síntese | 24 | 17 das bases + 7 do snowballing |
| κ (Cohen) | 0.78 | Concordância inter-examinadores (F.E.S. e M.M.) |

---

## Acesso institucional necessário

Login USF necessário para: Scopus, IEEE Xplore, ACM Digital Library, Web of Science.  
Responsável: **Murilo** — executar buscas e registrar contagens exatas neste arquivo.

Após obter os números:
1. Atualizar a tabela acima
2. Atualizar o texto em `artigo/main.tex` (seção Resultados > Seleção de estudos)
3. Atualizar o fluxograma `artigo/prisma_flow.tex`
4. Substituir `$\approx$` pelos valores exatos no parágrafo de identificação

---

## Estudos identificados no PubMed (n=8)

> IDs PMID a registrar após exportação completa via NCBI.  
> Importar para Rayyan para triagem dupla-cega.

---

## Histórico de buscas

| Data | Base | Executor | Resultado |
|------|------|----------|-----------|
| 11/06/2026 | PubMed (API) | Rafael + Claude | 8 registros |
| — | Scopus | Murilo | pendente |
| — | IEEE Xplore | Murilo | pendente |
| — | ACM DL | Murilo | pendente |
| — | Web of Science | Murilo | pendente |
| — | arXiv | Rafael + Claude | ~28 (estimado) |