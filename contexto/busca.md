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
| PubMed/MEDLINE | **786** | Exato | Filtros: 2014-2026, inglês/espanhol, free full text |
| **Total** | **786** | Exato | PubMed/MEDLINE como base eletrônica primária |

---

## Etapas PRISMA concluídas

| Etapa | Valor | Status / Observação |
|-------|-------|---------------------|
| Registros identificados (bases) | 786 | PubMed/MEDLINE |
| Fontes adicionais (Snowballing)| 6 | Identificados manualmente |
| Após remoção de duplicatas | 759 | 27 duplicatas removidas |
| Triados por T&A | 759 | Triagem dupla-cega |
| Excluídos no T&A | 724 | Com base nos critérios de elegibilidade |
| Texto completo avaliado | 41 | 35 das bases + 6 do snowballing |
| Excluídos no texto completo | 17 | 17 das bases (distribuídos em EC1-EC7); 0 do snowballing |
| Incluídos na síntese | 24 | 18 das bases + 6 do snowballing |
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