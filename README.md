📊 Painel Estratégico de Gestão de Estoque - LLC Eletronics

Este projeto consiste na estruturação e análise de dados de estoque para a LLC Eletronics, transformando planilhas dispersas em um painel gerencial consolidado no Excel. O objetivo é permitir que o time de operações visualize gargalos, controle saldos e tome decisões baseadas em dados confiáveis.

O projeto abrange desde a limpeza e relacionamento de dados até a criação de dashboards interativos com Tabelas Dinâmicas.

📸 Visualização do Projeto

1. Dashboard Gerencial (Painel Final)

Visão consolidada com indicadores de valor em estoque, movimentação e alertas de status.

<img width="1269" height="869" alt="Screenshot 2025-11-25 234812" src=  />

<img width="1269" height="869" alt="Screenshot 2025-11-25 234812" src=  />

2. Estrutura de Dados e Modelagem

Para garantir a integridade da análise, os dados foram estruturados em tabelas relacionais e tabelas dinâmicas.

Aba Resumo de Estoque (Tratamento de Dados):
Aqui foram aplicadas as funções PROCV, SOMASES e as lógicas de Status.
(Substitua pelo print da sua aba de tabelas/cálculos)

Tabela Dinâmica (Motor de Cálculo):
A estruturação que alimenta os gráficos e permite a interatividade do painel.
(Substitua pelo print da sua tabela dinâmica)

🎯 Objetivo do Desafio

Como analista de dados, a missão foi resolver a desorganização do controle de estoque, que dificultava o acompanhamento de entradas e saídas. As principais metas foram:

*  Consolidação: Unificar dados de cadastro, entradas e saídas.

* Automação: Calcular saldos e status automaticamente para evitar erros manuais.

*  Visibilidade: Criar um painel visual para reuniões estratégicas.

*  Gestão de Risco: Identificar produtos obsoletos, críticos ou com estoque negativo.

🛠️ Etapas de Desenvolvimento e Soluções Técnicas

O projeto foi dividido em 4 fases estratégicas para garantir integridade e usabilidade:

1. Relacionamento e Tratamento de Dados

Criação da aba matriz Resumo Estoque unificando as fontes.

*  Técnicas: Uso de PROCV (ou XLOOKUP) para buscar categorias e preços.

*  Cálculos: Utilização de SOMASES para totalizar entradas e saídas por SKU, garantindo que o saldo (Entradas - Saídas) reflita a realidade.

*  Valorização: Cálculo do Valor em Estoque (Saldo * Preço Unitário) para visão financeira.

2. Lógica de Status e Classificação

Implementação de regras de negócio para categorizar a saúde do estoque automaticamente:

*  Fórmulas: Uso de funções lógicas aninhadas (SE, E, IFS) para determinar o Status do Produto.

*  Regras:

        soleto: Estoque zerado.

        Crítico: Saldo entre 1 e 20 unidades.

        OK: Saldo saudável (21 a 100).

        Excesso: Acima de 100 unidades (custo de oportunidade).

        Negativo: Atenção imediata (erro operacional).

3. Visualização e UX (User Experience)

Foco na usabilidade da planilha para o usuário final.

  *  Formatação Condicional: Alertas visuais automáticos (Vermelho para negativo, Verde para positivo) para facilitar a leitura rápida.

  *  Validação de Dados: Listas suspensas para padronizar a entrada de categorias, evitando erros de digitação.

  *  Design: Congelamento de painéis e padronização de cabeçalhos.

4. Inteligência de Negócio (Dashboard)

Construção do painel final utilizando Tabelas Dinâmicas.

            Gráfico/Análise                                  Objetivo Estratégico                              Tipo de Visualização

    Capital Alocado por Categoria    Identificar onde o dinheiro da empresa está parado ou investido.            Colunas Agrupadas

    Movimentação de Saída            Mostrar quais categorias têm maior giro (demanda).                          Barras Horizontais

    Ticket Médio por Categoria       Comparar o valor agregado dos produtos.                                     Colunas Verticais

🧠 Insights e Tomada de Decisão

A partir do painel construído, o gestor pode responder a perguntas críticas:

🚨 Gestão de Risco

Identificação: Quais produtos estão com estoque negativo?

Ação: Investigar falhas de registro ou perdas físicas imediatamente.

💸 Eficiência Financeira

Identificação: Qual categoria concentra o maior valor em estoque parado (Excesso)?

Ação: Criar promoções para liberar capital de giro.

📦 Planejamento de Compras

Identificação: Quais produtos estão com status "Crítico" e alta saída?

Ação: Priorizar a reposição urgente para evitar ruptura de vendas (Stockout).

👤 Autor

Projeto Desenvolvido por: Fábio R Soares
