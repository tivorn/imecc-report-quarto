# imecc-report

Extensão Quarto para relatórios acadêmicos do IMECC — Unicamp, em conformidade com as normas ABNT (NBR 14724).

## Instalação

```bash
quarto use template <repo-url>
```

## Uso

No YAML do seu arquivo `.qmd`:

```yaml
format: imecc-report-pdf
```

### Metadados disponíveis

| Campo | Descrição | Padrão |
|-------|-----------|--------|
| `title` | Título do relatório | — |
| `author` | Nome do autor | — |
| `local` | Local (cidade) | `"Campinas"` |
| `ano` | Ano | Ano atual |
| `resumo` | Texto do resumo (opcional) | — |
| `palavras-chave` | Palavras-chave separadas por ponto (opcional) | — |
| `lista-siglas` | Itens `\item[SIGLA] Descrição` (opcional) | — |
| `lista-simbolos` | Itens `\item[$\alpha$] Descrição` (opcional) | — |

### Ambientes LaTeX

A extensão fornece os ambientes `resumo-pt`, `resumo-en` e `citacao` via filtro `latex-environment`.

## Licença

MIT
