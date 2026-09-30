Sobre o projeto
Aplicação para um trabalho de faculdade que compara a chuva com os níveis dos reservatórios e mostra cenários de risco de falta de água em Minas Gerais.
O estudo usa quatro reservatórios: Furnas, Emborcação, Três Marias e Irapé. Esses locais não representam todo o estado.
Funcionalidades
- Painel com o índice de risco atual.
- Histórico de chuva e níveis dos reservatórios.
- Comparação por região, ano e mês.
- Gráficos para visualizar os dados.
- Simulações de 2027 a 2035, considerando mudanças na chuva e na população.
- Explicação dos cálculos e das fontes utilizadas.
Tecnologias
- HTML5
- CSS3
- JavaScript puro
- JSON
- Chart.js 4.4.8
Toda a aplicação está em um único arquivo HTML, incluindo os dados e os gráficos. Não precisa de instalação e funciona sem internet.
Fontes de dados
- Open-Meteo: chuva de janeiro de 2020 a agosto de 2026, usando a base ERA5 do Copernicus/ECMWF. Atribuição Open-Meteo e Copernicus/ECMWF, licença CC BY 4.0.
- ONS: níveis diários dos reservatórios de 2020 a 2026. A leitura mais recente incluída é de 28/09/2026.
- IBGE: população estimada de Minas Gerais, conforme as Projeções da População, revisão 2024.
Os dados estão salvos no HTML e não são atualizados automaticamente.
Como o risco é calculado
O índice vai de 0 a 100 e usa os seguintes pesos:
- Chuva: 45%.
- Nível do reservatório: 45%.
- Crescimento populacional: 10%.
O índice geral é a média dos quatro locais. As faixas são:
Índice	Risco	Cor
0 a 20	Baixo	Verde
Acima de 20 até 40	Moderado	Amarelo
Acima de 40 até 60	Elevado	Laranja
Acima de 60 até 80	Alto	Vermelho
Acima de 80 até 100	Crítico	Vinho
