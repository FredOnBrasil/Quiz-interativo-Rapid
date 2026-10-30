# RAPID Challenge — ABB IRC5

[![Robotics](https://img.shields.io/badge/Domain-Industrial%20Robotics-0052cc.svg)](https://new.abb.com/products/robotics)
[![Language](https://img.shields.io/badge/Language-RAPID%20%7C%20HTML5%20%7C%20JS-blue.svg)](#)
[![Target](https://img.shields.io/badge/Target-Postgraduate%20%2F%20Specialization-success.svg)](#)

Uma plataforma interativa web para avaliação e fixação de conceitos avançados de programação em **linguagem RAPID** para controladores **ABB IRC5**. Desenvolvida como material didático e ferramenta de avaliação contínua para a disciplina de **Sistemas Robotizados** em cursos de Especialização e Pós-Graduação em Robótica Industrial e Automação.

---

## 📋 Sumário

- [Visão Geral](#-visão-geral)
- [Objetivos Pedagógicos](#-objetivos-pedagógicos)
- [Estrutura dos Módulos](#-estrutura-dos-módulos)
- [Características e Funcionalidades](#-características-e-funcionalidades)
- [Fundamentação Técnica e Referências](#-fundamentação-técnica-e-referências)
- [Como Utilizar](#-como-utilizar)
- [Integração Acadêmica e Avaliação](#-integração-acadêmica-e-avaliação)

---

## 🎯 Visão Geral

O **RAPID Challenge** coloca o estudante no papel de um engenheiro/especialista de robótica responsável pela auditoria, diagnóstico e validação de rotinas de código RAPID. 

Em vez de testar a simples memorização de sintaxe, o desafio foca no **raciocínio crítico sobre o comportamento físico e operacional do robô** frente às instruções programadas, abordando cenários reais de aplicação industrial (como células de montagem, *Pick and Place*, manipulação e usinagem/acabamento).

---

## 🎓 Objetivos Pedagógicos

No contexto da especialização em **Sistemas Robotizados**, a aplicação visa desenvolver as seguintes competências técnicas:

1. **Interpretação e Análise Crítica de Código:** Capacidade de ler e diagnosticar programas RAPID identificando potenciais falhas de lógica, colisões ou movimentos indesejados.
2. **Diferenciação de Estruturas de Dados e Tipos de Movimento:** Compreensão profunda das diferenças conceituais entre trajetórias articulares (`MoveJ`), lineares (`MoveL`) e circulares (`MoveC`), bem como o impacto de `robtarget`, `tooldata`, `wobjdata`, `speeddata` e `zonedata`.
3. **Sincronização Física x Lógica de I/O:** Conscientização sobre a diferença vital entre emitir um comando digital (`SetDO`) e confirmar o estado físico do processo via sensores (`WaitDI`), prevenindo falhas de colisão ou manipulação indevida.
4. **Segurança e Robustez Operacional:** Aplicação de boas práticas na estruturação de rotinas, controle de configuração do robô (`ConfJ`/`ConfL`), tratamento de exceções, paradas de emergência e validação gradual de trajetórias.

---

## 📚 Estrutura dos Módulos

O quiz é composto por **30 questões de análise**, distribuídas em **6 módulos temáticos**:

| Módulo | Escopo do Módulo | Tópicos Chave |
| :--- | :--- | :--- |
| **1. Fundamentos da Linguagem RAPID** | Declaração e escopo de dados, rotinas e mensagens ao operador. | `VAR`, `CONST`, `PERS`, `PROC` vs. Funções, `TPWrite`, operadores (`:=`, `<>`). |
| **2. Movimentação e Trajetória** | Cinemática de movimento, interpolação e perfis de trajetória. | `MoveJ`, `MoveL`, `MoveC`, zona de aproximação (`zonedata`), paradas exatas. |
| **3. Dados e Referências** | Geometria, referenciais de trabalho e cargas do manipulador. | `robtarget` (quaterniões/configuração), `tooldata` (TCP), `wobjdata`, `speeddata`. |
| **4. I/O e Sincronização** | Comunicação com periféricos, sensores e intertravamentos de segurança. | `SetDO`, `Reset`, `WaitDI`, `WaitTime` vs. sinais físicos, condições de permissivo. |
| **5. Lógica, Repetição e Temporização** | Controle de fluxo de execução da aplicação. | `IF`/`ELSE`, laços `WHILE`, laços `FOR`, condições lógicas compostas (`AND`/`OR`). |
| **6. Robustez, Diagnóstico e Boas Práticas** | Dinâmica, configuração articular e segurança operacional. | `GripLoad`, `ConfJ`/`ConfL`, `StopMove` vs `Stop`, estratégias de tratamento de falha. |

---

## ⚡ Características e Funcionalidades

- **Embaralhamento Dinâmico (Anti-Viés):** Algoritmo *Fisher-Yates* integrado via JavaScript que embaralha aleatoriamente as opções de resposta a cada tentativa, garantindo que a resposta correta não fique fixada na primeira posição e promovendo o aprendizado contínuo.
- **Feedback Pedagógico Imediato:** Explicações fundamentadas tecnicamente são exibidas logo após a seleção da resposta, indicando não apenas o erro/acerto, mas a razão teórica e prática.
- **Sistema de Dicas (*Hints*):** Dicas conceituais disponíveis para guiar o raciocínio do estudante antes da tomada de decisão.
- **Relatório Detalhado de Desempenho:** Gráficos e métricas com o aproveitamento percentual do aluno por módulo temático ao final do desafio.
- **Emissão de Certificado Digital:** Geração dinâmica de certificado de conclusão local com opção otimizada para **impressão ou exportação em PDF**, facilitando a entrega de trabalhos na plataforma acadêmica (ex.: Google Classroom, Moodle).
- **Execução Offline/Local:** Arquivo único em HTML5/CSS3/JavaScript puro (Single Page Application - SPA), podendo ser executado em qualquer navegador sem necessidade de servidor ou conexão com a internet.

---

## 📖 Fundamentação Técnica e Referências

O conteúdo técnico das questões e explicações do sistema foi elaborado e rigorosamente alinhado com a documentação oficial da **ABB Robotics**:

- **Manual de Referência:** *RAPID Instructions, Functions and Data types*
- **Versão do RobotWare:** RobotWare 6.06
- **Código do Documento ABB:** `3HAC050917-001`, Revisão F

---

## 🚀 Como Utilizar

1. **Acesso Direto:**
   - Faça o download do arquivo `rapid_challenge_abb_irc5_avancado.html`.
   - Abra o arquivo em qualquer navegador web moderno (Chrome, Firefox, Edge, Safari).

2. **Realização da Atividade:**
   - Leia as instruções na tela inicial de **Missão**.
   - Responda às 30 questões prestando atenção aos detalhes técnicos do código fornecido.
   - Analise os *feedbacks* exibidos para consolidar a fundamentação teórica.

3. **Geração do Comprovante de Conclusão:**
   - Ao terminar o quiz e obter o aproveitamento mínimo recomendado (≥70%), clique em **Gerar certificado**.
   - Digite seu nome completo no campo indicado.
   - Clique em **Imprimir / salvar como PDF** e salve o arquivo gerado para envio ao professor/plataforma acadêmica.

---

## 🏫 Integração Acadêmica e Avaliação

### Sugestão de Uso pelo Professor/Instrutor:
- **Atividade Pré/Pós-Laboratório:** Utilizar o quiz após as aulas teóricas de RAPID para preparar os alunos antes das práticas no robô real ou no software *ABB RobotStudio*.
- **Avaliação Formativa:** Analisar o desempenho nos módulos para identificar quais tópicos (como *Frames/WObj*, *TCP* ou *Intertravamentos*) necessitam de reforço em sala de aula.
- **Metodologia Ativa:** Utilizar as questões mais complexas como estudos de caso para discussão em grupo sobre diagnósticos de falha na célula robotizada.

---

*Material desenvolvido para apoio ao ensino de Robótica Industrial e Programação de Robôs Articulados.*
```

eof

### Resumo das atualizações:
- O arquivo `README.md` foi estruturado profissionalmente com foco na **Especialização em Sistemas Robotizados**.
- O documento descreve a aplicação, os objetivos pedagógicos, o escopo técnico do manual ABB IRC5 (RobotWare 6.06) e detalha a implementação do algoritmo de **embaralhamento dinâmico** que corrigiu o viés da primeira opção.