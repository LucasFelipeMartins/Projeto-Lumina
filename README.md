# Plataforma Híbrida de Gestão de Saúde, Nutrição e Treino

![Status](https://img.shields.io/badge/Status-Fase_de_Engenharia_e_Design-orange)
![Tipo](https://img.shields.io/badge/Tipo-TCC_%7C_Trabalho_Acadêmico-blue)
![Artefatos](https://img.shields.io/badge/Artefatos-UML_%7C_Protótipos_%7C_Métricas-brightgreen)

## Visão Geral

Este repositório documenta a fase de Engenharia de Software e Design de Interface do meu Trabalho de Conclusão de Curso (TCC). O projeto conceitua uma plataforma inteligente que unifica a gestão de exames médicos, planos nutricionais e fichas de treinamento físico. 

O grande diferencial arquitetural planejado é a **Gestão Híbrida**: o sistema foi modelado para utilizar um **Motor de Regras de Inteligência Artificial** na geração de pré-análises, que são posteriormente validadas e ajustadas por **Profissionais Humanos** (Nutricionistas, Educadores Físicos e Médicos).

> **Aviso:** No momento, este repositório contém exclusivamente a **modelagem do sistema (diagramas UML)** e os **protótipos de interface (UI/UX)**. O código-fonte da aplicação será desenvolvido em etapas futuras.

## Estrutura do Repositório

* `Diagramas` - Contém todos os diagramas arquiteturais e comportamentais gerados para o projeto.
* `PrototipacaoInterface` - Telas, wireframes e fluxos de navegação (UI/UX).
* ` docs/metricas/ ` - Relatórios de estimativa de esforço e tamanho do software.

## Engenharia de Software e UML

A arquitetura do sistema foi rigorosamente documentada para garantir alta coesão e baixo acoplamento antes da implementação. Os seguintes artefatos estão disponíveis:

* **Diagrama de Classes:** Estruturação orientada a objetos (Perfis, Relatórios Base, Interfaces de Gestores).
* **Diagrama de Casos de Uso:** Mapeamento das interações entre o Paciente, o Profissional Humano e o Motor de IA.
* **Diagramas de Atividades:** Modelagem detalhada das *Regras de Negócio* (Filtros de orçamento, cruzamento de lesões e recálculo de rotas metabólicas).
* **Diagrama de Máquina de Estados:** O ciclo de vida completo do "Plano Integrado", desde o rascunho até a ativação, revisão e arquivamento.
* **Diagrama de Implantação:** Topologia de nuvem projetada, separando nós de banco de dados, API principal e Servidor de Inteligência Artificial isolado.

##  Prototipação e Interface (UI/UX)

A experiência do usuário foi desenhada para facilitar a jornada do paciente (inserção de exames e acompanhamento visual) e otimizar o tempo do profissional de saúde (dashboard de aprovação de dietas/treinos).

## Escopo Funcional Modelado

A modelagem atual prevê a construção dos seguintes módulos principais:

### Módulo do Paciente
* Cadastro de métricas corporais e histórico de doenças.
* Gestão de Exames (upload de laudos e comparativo de evolução - Massa Magra vs. Gordura).
* Sistema de Lembretes configuráveis (hidratação, refeições e treinos).

### Módulo do Gestor Híbrido (IA & Profissional)
* Motor de Geração de Dieta: Cruzamento de exames, alergias e orçamento.
* Prescrição Esportiva: Recomendação de modalidades e seleção de exercícios filtrados por limitações físicas.
* Painel de Validação: Interface de auditoria clínica.

## Métricas de Software e Planejamento (PCU)

Para garantir a viabilidade acadêmica e de execução do projeto, o escopo foi estimado matematicamente utilizando a metodologia de **Pontos de Caso de Uso (Karner, 1993)**:

* **Tamanho Base Bruto (PCUNA):** 88 Pontos (Baseado em 3 Atores e 9 Casos de Uso centrais).
* **Fatores de Ajuste (FCT/FCA):** Ponderação baseada no uso de motor de regras complexo, requisitos de segurança de dados de saúde e ambiente acadêmico.
* **Tamanho Ajustado Final:** 74,58 PCUA.
* **Esforço de Codificação Estimado:** ~1.490 horas de trabalho (Projeção: execução viável em ~4,5 meses por uma dupla de desenvolvedores).

##  Próximos Passos

1. Validação dos protótipos de interface com usuários beta.
2. Definição da stack tecnológica oficial (Frontend, Backend e Banco de Dados).
3. Início da codificação (Módulo de Autenticação e Perfis Base).

## Licença
Este projeto está sob a licença MIT. Feito para fins acadêmicos e de pesquisa (Trabalho de Conclusão de Curso).
