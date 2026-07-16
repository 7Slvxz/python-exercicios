# 🏫 Sistema de Gerenciamento de Histórico Escolar

Aplicação interativa desenvolvida em Python voltada para o gerenciamento de desempenho acadêmico de alunos. O sistema permite cadastrar múltiplas disciplinas, coletar e validar notas e frequências, calcular médias e emitir um relatório completo de situação do estudante (Aprovado, Reprovado por Falta ou Recuperação).

## 📈 Evolução do Projeto e Aprendizado Incremental

Este projeto foi desenvolvido de forma modular e evolutiva ao longo do primeiro semestre da faculdade. O código foi refatorado e expandido a cada novo conceito absorvido, dividindo-se nas seguintes fases de engenharia:

1. **Fase Sequencial:** Estruturação inicial do fluxo do programa, entrada e saída de dados de forma linear.
2. **Fase de Decisão:** Implementação de estruturas condicionais (`if`, `elif`, `else`) para determinar de forma automática a situação final do aluno com base nas regras de negócio.
3. **Fase de Repetição:** Adicionados laços dinâmicos (`while` e `for`) para permitir o cadastro contínuo de matérias, além de criar rotinas rígidas de validação de dados.
4. **Estruturas de Dados:** Implementação de coleções lógicas (Listas e Matrizes dinâmicas) para armazenar todo o histórico de dados em memória e gerar um relatório final consolidado.

## 🚀 Funcionalidades Técnicas

* **Menu Interativo Continuável:** Permite que o usuário cadastre quantas disciplinas desejar em uma única execução através do controle de fluxo por laço `while`.
* **Validação de Entrada de Dados (Data Cleansing):** O sistema impede o avanço se o usuário digitar notas fora do intervalo de `0.0 a 10.0` ou frequências fora de `0 a 100%`.
* **Cálculo Automatizado:** Processamento aritmético para extrair a média das 4 notas bimestrais e a média de presença do período.
* **Lógica de Situação Acadêmica (Regras de Negócio):**
  * **Aprovado:** Nota média $\ge$ 5.0 e frequência $\ge$ 70%.
  * **Reprovado por Falta:** Frequência inferior a 70% (critério eliminatório).
  * **Recuperação:** Frequência regulamentada ($\ge$ 70%), porém nota média inferior a 5.0.
* **Persistência de Dados em Memória e Relatório Final:** Uso do método `.append()` para construir uma matriz dinâmica contendo o histórico de cada disciplina, desempacotada ao final da execução em um resumo limpo para o usuário.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Paradigma:** Programação Estruturada
* **Ambiente de Desenvolvimento:** Jupyter Notebook (`.ipynb`) / Anaconda Environment

## 📁 Estrutura do Arquivo

```text
├── PROJETOESCOLA/
│   └── code.ipynb   <-- Código-fonte comentado e documentado
└── README.md        <-- Documentação técnica do projeto
