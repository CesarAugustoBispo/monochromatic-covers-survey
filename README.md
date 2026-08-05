# Monochromatic Covers Survey

Survey de literatura sobre **cobertura e partição em estruturas monocromáticas** em grafos com coloração de arestas.

## Tema

Dado um grafo com arestas coloridas com $r$ cores, o objetivo é cobrir ou partir os vértices usando cópias monocromáticas de estruturas como **caminhos**, **ciclos**, **árvores** ou **componentes conexas**.

Classes de grafos estudadas:
- Grafos completos ($K_n$)
- Grafos com grau mínimo alto ($\delta(G) \geq 3n/4$, $2n/3$, etc.)
- Grafos aleatórios $G(n,p)$
- Grafos bipartidos ($K_{n,n}$)
- Grafos multipartidos ($K_{n_1,\ldots,n_s}$)

## Conjecturas centrais

| Conjectura | Status |
|---|---|
| **Gyárfás** — $r$ caminhos cobrem $K_n$ $r$-colorido | Aberta para $r \geq 4$ |
| **Erdős–Gyárfás–Pyber** — $r$ ciclos particionam $K_n$ | Falsa para $r \geq 3$ (Pokrovskiy 2014) |
| **Lehel** — 2 ciclos cobrem $K_n$ 2-colorido | Provada (Bessy–Thomassé 2010) |
| **Ryser** — $r-1$ classes cobrem hipergrafos $r$-partidos | Aberta para $r \geq 4$ |

## Arquivos

| Arquivo | Descrição |
|---|---|
| `survey_v1.tex` | Livro LaTeX com enunciados, contexto histórico e problemas abertos (bilíngue) |
| `survey_v2.tex` | Versão com esboços de provas e caixas de técnicas |
| `lista_papers.txt` | Lista dos 44 artigos organizados por tema |
| `papers/*.pdf` | PDFs baixados do arXiv (44 artigos) |

## Compilando

```bash
pdflatex survey_v1.tex
pdflatex survey_v1.tex   # segunda passagem para TOC/refs

pdflatex survey_v2.tex
pdflatex survey_v2.tex
```

Requer: `texlive` com pacotes `mdframed`, `tcolorbox`, `hyperref`, `lmodern`.

## Papers

44 artigos cobrindo o período 2012–2026. Técnicas principais:

- Regularity Lemma (Szemerédi)
- Método de matchings conexos (Łuczak)
- Método de absorção
- Blow-up Lemma
- Método probabilístico / Lovász Local Lemma

## Contexto

Material organizado para qualificação de doutorado em Teoria dos Grafos / Combinatória.
