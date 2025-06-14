# Desafio Imposto de Renda DIO

## ⛓️ BASE ESTRUTURAL

## 📋 — 1. Sobre o Projeto

Este projeto foi desenvolvido como uma planilha interativa voltada para a análise financeira, permitindo aos usuários simular e organizar sua declaração de Imposto de Renda de forma eficiente. A proposta central envolve o uso de fórmulas e formatação condicional para aprimorar a visualização de rendimentos, informes bancários e valores recebidos mensalmente. Além disso, a planilha conta com um sistema integrado de informes e notas, possibilitando a entrada e saída de valores de maneira intuitiva. Com a inclusão de um totalizador de valor restante, os usuários podem acompanhar suas finanças em tempo real, facilitando a tomada de decisões e proporcionando maior clareza na gestão do patrimônio.

## 📊 — 2. Qual a estrutura da planilha?

A planilha apresenta três tópicos controlados dinâmicamente pelo menu criado na coluna `A`, mas por botões de acesso entre as célular `A11;A12` até `A17;A18` estruturados para:

- **Dados do Titular:** O usuário através do preenchimento de seus dados de pessoa física, consegue ter um acompanhamento fixo que vai de seu nome até dados condicionais em menu sobre se há alterações em seu cadastro, dependentes ou se atualmente reside no exterior, dando um controle maior sobre suas informações para futuras alterações;

- **Informes de Rendimentos Bancários:** O sistema de Informes de Rendimentos Bancários proporciona uma visão centralizada e organizada dos saldos disponíveis em diferentes instituições financeiras. Através de um menu interativo, o usuário pode selecionar o banco desejado e registrar o valor atual em conta, garantindo um acompanhamento preciso dos recursos distribuídos entre diversas instituições;

- **Notas Bancárias e/ou Extratos de Holerites:** O sistema de Notas Bancárias e Extratos de Holerites organiza as movimentações financeiras do usuário, permitindo a classificação de entradas por CNPJ, Freelance ou Holerite, individualmente, com registro de valores e datas. As despesas são categorizadas conforme o destino dos gastos, facilitando o controle financeiro. Um totalizador automático subtrai os valores recebidos dos gastos, proporcionando um saldo atualizado e uma visão clara das finanças;

### 2.1. Amostra de dados (Informes):

![image](https://github.com/user-attachments/assets/573882ff-8eb9-4fe2-82f3-b959eeb2658b)

### 2.2. Amostra de dados (Notas):

![image](https://github.com/user-attachments/assets/963fd310-2bd9-463a-91f8-76380c83e9bd)

---

## ⚜️ CONTEXTO FOCAL

## 📉 — 3. Menu de Escolha (na coluna `A`):

- **Menu Titular** – Local onde se faz o preenchimento dos dados da pessoa fisica;
- **Menu Informes** – Local onde se preenche com dados atuais de cada banco;
- **Menu Notas** – Local onde se concentram os valores de entrada mês a mês de receita e gastos;

### 3.1. Construção do Modelo (Titular):
É onde se preenchem os dados da pessoa fisica, com maior controle e estabilidade de validação de informações.

- Se baseia no sistema de Nome, CPF, Nascimento, Rua, CEP, Telefone, entre outros. Ainda deixando em aberto a possibilidade de anunciar se houve alteração em cadastro ou não, assim como uma possível mudança de residência para o exterior;

### 3.2. Construção do Modelo (Informes):
É onde se preenche com dados atuais de cada banco de maneira unificada por partes individuais.

- As colunas `C` e `D` analisam o banco (escolhido manualmente pelo sistema de lista), ao qual o usuário agrega o valor atual em conta e, o arquivo em anexo do comprovante;
- Através da célula `D23` chegamos ao total que há em conta pela somatória das células `D8`, `D14` e `D20`;

### 3.3. Construção do Modelo (Notas):
É onde todos os valores de entrada mês a mês de receita se encontram, juntamente as despesas e o saldo restante.

- Na linha `6` enquanto a coluna `C` a partir de estabelece de `C8` até `C15` as datas de entrada, temos na coluna `D` estruturando de `D8` até `D15` a escolha da categoria, sendo de CNPJ, Freelance ou Holerite para maior acessibilidade e, por fim, na coluna `E` encontramos os valorea a serem despostos nas mesmas células de `E8` até `E15` dos valores em entrada;
- Através das mesmas colunas, mas na linha `18`, temos nas mesmas proporções, mas de `20` até `27`, onde na coluna `D` agora encontramos as principais despesas, como Moradia, Saúde, Alimentação, Lazer, Educação, entre outros;
- Ao fim, encontramos um sistema de gastos totais onde há o valor total de entrada, da somatória dos mêses pela subtração dos gastos nesses mesmos mêses, proporcionando um saldo claro de valor restante dentro do período;

---

## 📍 CONCLUSÃO

## 📈 — 4. Proposta da Planilha

- **Gestão Financeira Interativa:** Através da Simulação e organização da declaração do Imposto de Renda permitir a visualização aprimorada dos rendimentos, informes bancários e valores recebidos mensalmente através de um sistema dinâmico de menus para facilitar o acesso às informações financeiras;
- **Validação e Organização de Dados:** Utilizar a validação de dados por listas, permitindo categorizar investimentos e despesas em um sistema de informes e notas que unifique registros organizados e acessíveis. Ademais, fomentando em um planejamento estratégico com projeções ajustáveis conforme as necessidades do usuário;
- **Controle de Entradas, Gastos e Saldo Restante:** Pelo uso da Fórmula SOMA aplicada para cálculos automáticos de receitas e despesas, construir um apoio visual para saber o quanto há de entrada e saída de valores, garantindo acompanhamento em tempo real. Dessa forma, se acompanha de totalizador de valor restante, proporcionando maior clareza na gestão patrimonial;

## ✖️ — 5. Construção

- Microsoft Excel;
- Fórmula SOMA;
- Sistema Interativo e Dinâmico de Menus;
- Sistema de Entrada & Gastos com Saldo restante;
- Validação de Dados por listas;
  
## 📂 — 6. Anexo do Arquivo
[Clique aqui para baixar](https://github.com/EdBerriel/Imposto-Renda-DIO/blob/main/Imposto%20de%20Renda%20DIO.xlsm)
