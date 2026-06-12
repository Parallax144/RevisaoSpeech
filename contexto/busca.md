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
| PubMed/MEDLINE | **8** | Exato | API NCBI E-utilities, 11/06/2026 |
| Scopus | ~275 | Estimado | Requer acesso institucional USF |
| IEEE Xplore | ~125 | Estimado | Requer acesso institucional USF |
| ACM Digital Library | ~50 | Estimado | Requer acesso institucional USF |
| Web of Science | ~200 | Estimado | Requer acesso institucional USF |
| arXiv | ~28 | Estimado | Busca direta (string simplificada) |
| **Total** | **~686** | Estimado | Exato: 8 (PubMed) + estimados demais |

---

## Etapas PRISMA pendentes

| Etapa | Valor | Aguarda |
|-------|-------|---------|
| Após remoção de duplicatas | [N] | Buscas institucionais + Rayyan |
| Triados por T&A | [N] | Idem |
| Excluídos no T&A | [N] | Triagem F.E.S. + M.M. |
| Texto completo avaliado | [N] | Triagem F.E.S. + M.M. |
| Excluídos no texto completo | [N] | Triagem F.E.S. + M.M. |
| Incluídos na síntese | [N] | Gate 2 |
| κ (Cohen) | [valor] | `irr::kappa2()` após triagem dupla-cega |

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