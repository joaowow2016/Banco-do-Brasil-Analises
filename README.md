[README.md](https://github.com/user-attachments/files/34765652/README.md)
# Banco do Brasil · Investigação OSINT dos resultados

Dashboard estático e interativo sobre o resultado do Banco do Brasil no 3T26, com indicadores históricos selecionados de 2010 a 2026. A investigação utiliza fontes públicas e registra hipóteses, evidências e limites de comparabilidade.

## Abrir o dashboard

Abra `index.html` em um navegador moderno. O painel funciona sem servidor; os links para as fontes externas exigem conexão.

Para publicar no GitHub Pages após enviar os arquivos para a branch padrão: acesse **Settings → Pages → Build and deployment → Deploy from a branch**, selecione a branch padrão e a pasta `/ (root)`, e salve. Depois da publicação, o endereço esperado é `https://joaowow2016.github.io/Banco-do-Brasil-Analises/`.

## Arquivos

- `index.html`: dashboard autônomo, com dados e estilos embutidos.
- `dados/series_limpas.csv`: indicadores históricos selecionados, com rastreabilidade até aba, célula e URL.
- `dados/dre_gerencial_2025_2026.csv`: contas da DRE gerencial 1T25–3T26, em R$ milhões.
- `METODOLOGIA.md`: fontes, reconciliações, limitações e interpretação dos resultados.

## Limitações

Trata-se de uma análise exploratória, não de auditoria, perícia, prova de irregularidade ou recomendação de investimento. Não foram examinados integralmente os 617 documentos baixados. Comparações históricas estão sujeitas a mudanças de perímetro e de regras contábeis. Em particular, a inadimplência publicada originalmente para o 3T25 difere da série reapresentada na edição 3T26; consulte a metodologia.

A investigação se orienta pelo catálogo de recursos de *Open Source Intelligence Tools and Resources Handbook* (Bielska et al., 2020), fornecido pelo solicitante. O livro não integra este repositório.
