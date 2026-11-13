# Hinojosa OS

Dashboard de gestão (produção, indicadores, financeiro, qualidade, manutenção, desperdícios) e **PDCA da Direção**.
É uma app estática: um único `index.html` (tudo incluído, funciona sem servidor).

## Publicar no GitHub Pages
1. Criar um repositório (**privado** — os dados são internos) e carregar `index.html`, `pdca.json` e `.nojekyll`.
2. *Settings → Pages → Deploy from a branch → `main` / root*.
3. Nota: o GitHub Pages a partir de repositório privado exige plano pago (Team/Enterprise). Em alternativa, abrir o `index.html` localmente ou alojá-lo na intranet.

## PDCA da Direção (partilha)
- As ações ficam guardadas no browser de cada utilizador.
- Para partilhar com toda a direção: **Exportar JSON** → substituir `pdca.json` no repositório (commit). Quem abrir a app sem dados locais carrega esse ficheiro; **Carregar pdca.json** força a atualização.
- **Exportar CSV** gera o plano para Excel.
- Responsáveis pré-definidos: sergio.ferreira, vitor.santos, joao.campos, mario.david, augusto.tavares (@graphicleader.pt). Aceita também outros e-mails.

## Atualização semanal / mensal
| Dados | Fonte | Estado atual |
|---|---|---|
| Produção / Indicadores | `BD__2026.xlsx` + `Horas_Disponiveis_2026.xlsx` | até W45 (8 nov 2026) |
| Financeiro | `MM2026_REPORTING_CONSEJO_GL.xlsx` | Jan–Out |
| Qualidade | PDFs/Excel de FIIs e FIQs | PDFs até semana 43 |
| Manutenção (SAP) | export SAP | Jan–Abr (desatualizado) |

Regras: uptime = tiragem / Duração Final (BD); Pasaban = 104 h/semana; horas disponíveis = planeamento.
