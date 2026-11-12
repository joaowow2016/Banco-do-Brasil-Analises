# Investigação OSINT · Banco do Brasil, 3T26

Data de referência: 12/11/2026. A pergunta investigativa é por que o lucro ajustado do 3T26, divulgado em 11/11/2026, caiu. “EAD” foi interpretado como **análise exploratória de dados (EDA)**. O painel é autônomo: abra `dashboard_bb_osint.html` em um navegador moderno. Seus dados estão embutidos; links externos exigem internet.

## Achado principal e distinções

O BB registrou lucro ajustado de R$ 1.269,5 milhões no 3T26, contra R$ 3.784,9 milhões no 3T25, e custo do crédito de R$ 21.234 milhões. A DRE gerencial indica, na comparação anual: margem financeira bruta −R$ 383,3 milhões; custo do crédito −R$ 3.305,9 milhões; outras receitas/despesas operacionais −R$ 1.458,2 milhões; resultado não operacional −R$ 6,2 milhões; IR/CS +R$ 2.408,6 milhões; participações estatutárias +R$ 262,9 milhões; minoritários −R$ 33,1 milhões. A soma dessas variações exclusivas corresponde à queda de R$ 2.515,3 milhões do lucro ajustado. Arredondamentos podem causar diferenças de R$ 0,1 milhão.

Segundo o BB, a pressão de crédito reflete especialmente a inadimplência em parte do agro e reforços em empresas do atacado. Isso é uma explicação atribuída à administração, não uma quantificação causal por carteira. Os índices também evidenciam piora em PF. O custo de crédito inclui despesa de perda esperada e descontos, menos recuperação; não é sinônimo de despesa de perda esperada, nem de saldo de provisões, baixas ou inadimplência.

## Discrepância relevante entre edições

A planilha publicada com 3T25 mostra atraso superior a 90 dias de **4,93%** em 3T25. A edição publicada com 3T26 reapresenta o mesmo período a **4,51%**. O numerador é R$ 54.769,8 milhões em ambas; o denominador é respectivamente R$ 1.111.687,0 milhões e R$ 1.214.344,9 milhões. O motivo da diferença de denominador não foi estabelecido nesta investigação. O aumento de 1,57 ponto percentual até 6,08% usa exclusivamente a série retrospectiva de 3T26; não mistura edições.

Existe outra diferença na sobreposição de 2014: os índices de atraso da edição 4T14 superam os da edição 3T26 em aproximadamente 0,17–0,22 p.p. A linha do painel é interrompida entre 2013 e 2014 para evitar uma continuidade enganosa. Os dados vêm como publicados; não se presumiu o motivo da mudança.

## Procedimento e escopo

- O livro anexo *Open Source Intelligence Tools and Resources Handbook* (Bielska et al., 2020) foi consultado como catálogo de busca, pesquisa empresarial, análise e checagem (páginas 17, 113, 299 e 309). Os seus recursos não substituem a validação das evidências e não foram todos executados.
- Fontes escolhidas: sumários e séries históricas de RI do BB, análise de desempenho 3T26, material do BC sobre a resolução e reportagem com contexto setorial. Não foi feita investigação sobre indivíduos nem foram usadas fontes privadas.
- Este é um recorte exploratório: **não foram lidos nem auditados integralmente os 617 documentos armazenados no Drive**. A análise da DRE detalha as 28 linhas gerenciais publicadas de 1T25 a 3T26, sem pretensão de abranger todas as contas societárias e notas.
- O CSV de séries possui 394 observações de sete indicadores. Lucro ajustado e inadimplência total cobrem 1T10–3T26; os demais iniciam mais tarde. A série de lucro e a inadimplência total usam dados do arquivo 4T14 até 2013 e da planilha 3T26 a partir de 2014. Essas emendas não constituem validação de equivalência histórica.
- O CSV de DRE contém os sete trimestres de 2025–2026, 28 linhas e referência à linha original. Abas e células específicas das séries estão no CSV. Os arquivos foram obtidos diretamente das mesmas fontes públicas que alimentaram os pacotes do Drive.
- Valores em branco não são imputados; células numéricas foram extraídas conforme valores armazenados, sem arredondamento no cálculo. As células da DRE gerencial atual e da DRE com realocações histórica estão em reais e foram divididas por 1 milhão; a planilha 4T14 usada no histórico está em milhões. Variações percentuais no painel são (atual − base)/|base| e não são calculadas quando base = 0.
- No arquivo de 3T26, **DRE com Realocações**: linhas 6–33, colunas B–H; **DRE com Realocações (Res. 4720)**: linha 54; **Índices de Atraso**: linhas 9 e 24; **Cobertura de Crédito**: linhas 11, 19 e 27; **Índice de Basileia**: linha 55, multiplicada por 100 para exibição percentual. No arquivo de 4T14: **DRE Realocações** linha 52 e **Índices de Atraso** linha 15.
- Testes numéricos nos sete trimestres: margem financeira bruta + custo do crédito = margem financeira líquida; recuperação + despesa de perda esperada + descontos = custo do crédito; resultado antes da tributação + IR/CS + participações = lucro ajustado. Maior resíduo absoluto < 0,000001 R$ milhão.
- Fontes, perímetros, moeda nominal, efeitos de inflação e retrospectivas de cada indicador não são necessariamente equivalentes. A entrada em vigor da Resolução CMN 4.966 em 2025 altera a apuração das perdas esperadas. Não se pode decompor uma mudança histórica em efeito regulatório versus econômico com esta base.
- A análise identifica associações e mecanismos contábeis. Não estabelece fraude, responsável, intenção, causalidade econômica ou recomendação de investimento. Para investigação aprofundada: conciliar notas, efeitos fiscais, reclassificações e metodologia; comparar bancos pares, coortes de concessão, garantias e perdas por safra; testar cenários e hipóteses alternativas.

## Fontes e preservação

1. [BB: séries históricas 3T26](https://filemanager-cdn.mziq.com/published/5760dff3-15e1-4962-9e81-322a0b3d0bbd/6fdeb4de-9f66-4c93-b93c-29ddd733cde7). SHA-256 `d271e643f3ad6bbb81e586ba588745d4398ba60357ad5c97c3bef7eebb702619`.
2. [BB: séries históricas 4T14](https://api.mziq.com/mzfilemanager/d/5760dff3-15e1-4962-9e81-322a0b3d0bbd/2292817c-1b7d-4aa0-a0c5-3cc654d39c04?origin=2). SHA-256 `6df41acfbe5396d50c37a7b7be2afbb90e8fed07046b0725b42492d159fc2ef4`.
3. [BB: sumário 3T26](https://filemanager-cdn.mziq.com/published/5760dff3-15e1-4962-9e81-322a0b3d0bbd/0e3bf08c-f87e-4e9a-b013-191b564d84cf). SHA-256 `78a9d2b3a97040f69e7bcaa25ff5b9a5b629a8e4e171ca9dc4f65e280f490105`.
4. [BB: análise de desempenho 3T26](https://filemanager-cdn.mziq.com/published/5760dff3-15e1-4962-9e81-322a0b3d0bbd/b93e763e-674c-4ec2-8bbc-324ef8f0fe51). SHA-256 `0f6b72b6b3905c2e00533817243e962b65a8e56661ffcdfdc6133f2b582a30a9`.
5. [BB: sumário original 3T25](https://api.mziq.com/mzfilemanager/v2/d/5760dff3-15e1-4962-9e81-322a0b3d0bbd/7f3dfbac-fffb-275a-1574-ffcc13941ba6?origin=2) e [série original 3T25](https://api.mziq.com/mzfilemanager/v2/d/5760dff3-15e1-4962-9e81-322a0b3d0bbd/23d30455-5d81-27f0-e761-f52afbbf8636?origin=2).
6. [Banco Central: revisão das estatísticas de crédito em 2025](https://www.bcb.gov.br/content/estatisticas/hist_estatisticasmonetariascredito/202502_Texto_de_estatisticas_monetarias_e_de_credito.pdf).
7. [CNN Brasil: reportagem sobre estudo Cepea, 02/11/2026](https://www.cnnbrasil.com.br/agro/custo-dos-juros-da-divida-rural-sobe-191-em-quatro-anos-mostra-cepea/). Contexto secundário; não mede efeito específico no BB.
8. Livro anexo do usuário, *OSINT Tools and Resources Handbook* (2020), 510 páginas; recursos e links podem estar desatualizados.
