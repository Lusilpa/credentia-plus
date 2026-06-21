# 🎓 Credentia+

**Sistema Unificado de Credenciamento e Gestão Para Eventos Acadêmicos e Científicos**

[![C++](https://img.shields.io/badge/C++-17-blue.svg?logo=c%2B%2B)](https://isocpp.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Solução offline especializada para gestão de eventos acadêmicos de grande porte.**

---

## 📋 Sobre o Projeto

O **Credentia+** é um sistema desenvolvido em C++ para resolver os desafios de gestão de eventos acadêmicos na região Norte do Brasil, onde a infraestrutura de internet é limitada. 

Criado inicialmente para atender limitações do **ENCOENG da FUCAPI**, o sistema oferece uma alternativa **totalmente offline** aos sistemas comerciais dependentes de conectividade constante.

### 🎯 Problema Solucionado
* 📡 **Dependência de internet:** Elimina falhas em regiões com infraestrutura instável.
* 💸 **Custos proibitivos:** Alternativa viável para instituições educacionais.
* 📝 **Gestão manual:** Automatiza processos para eventos com centenas de participantes.
* 🎓 **Foco acadêmico:** Adequação específica para certificados, palestras e horas complementares.

---

## ✨ Funcionalidades

### 🏗️ Módulos Principais

| Módulo | Descrição | Funcionalidades Chave |
| :--- | :--- | :--- |
| **📅 Eventos** | Gestão completa do ciclo de vida | CRUD, credenciamento autônomo, controle de fluxo. |
| **👥 Participantes** | Cadastro de usuários | Validação de CPF, múltiplos telefones/cursos, instituições vinculadas. |
| **🎤 Palestrantes** | Gestão de convidados | Cadastro simplificado, vínculo com atividades, títulos acadêmicos. |
| **📚 Atividades** | Gestão de atividades paralelas | Check-in inteligente, lista de espera, controle de lotação. |
| **🏫 Instituições** | Cadastro institucional | Autenticação por ID/senha, múltiplos telefones de contato. |
| **📜 Certificados** | Emissão de documentos | Geração automática baseada no tipo de participação. |

### 🔧 Destaques Técnicos
* **✅ Validação de CPF:** Algoritmo recursivo oficial para verificação de dígitos.
* **💾 Persistência:** Sistema de arquivos texto (`.txt`) para operação offline.
* **🧠 Memória:** Alocação dinâmica com arrays e gestão manual de recursos.
* **📊 Modelagem:** Uso extensivo de Structs e Classes.
* **🔄 Check-in Dual:** Lógica de inscrição direta vs. lista de espera.
* **🎫 Credenciamento:** Interface de terminal autônoma por CPF.

---

## 🛠️ Tecnologias e Conceitos

### 🚀 Stack Tecnológico
* **Linguagem:** C++ (Standard C++17)
* **Persistência:** Arquivos de texto estruturados
* **Compilação:** Cross-platform (GCC, Clang, MSVC)

### 📚 Conceitos Acadêmicos Aplicados

| Conceito | Aplicação no Projeto |
| :--- | :--- |
| **Ponteiros e Alocação Dinâmica** | Arrays dinâmicos para listas de telefones e cursos. |
| **Structs e Classes** | Modelagem de entidades (Participante, Evento, Atividade). |
| **Recursividade** | Algoritmo de validação de dígitos do CPF. |
| **File I/O (Fstream)** | Banco de dados manual via leitura/escrita sequencial. |
| **Regra dos Três** | Gestão de memória (Construtor, Destrutor, Copy) em classes complexas. |
| **Modularização** | Separação estrita entre Interface (`.hpp`) e Implementação (`.cpp`). |

---

## 📦 Estrutura do Projeto

```text
Credentia/
├── include/                  # Cabeçalhos (.hpp)
│   ├── MainInterno.hpp
│   ├── Participante.hpp
│   ├── Evento.hpp
│   ├── AreaAtividades.hpp
│   ├── Palestrante.hpp
│   ├── Instituicao.hpp
│   ├── Certificados.hpp
│   └── ValidadorCPF.hpp
│
├── src/                      # Implementações (.cpp)
│   ├── MainInterno.cpp
│   ├── Participante.cpp
│   ├── Evento.cpp
│   ├── AreaAtividades.cpp
│   ├── Palestrante.cpp
│   ├── Instituicao.cpp
│   ├── Certificados.cpp
│   └── ValidadorCPF.cpp
│
├── data/                     # Persistência (.txt)
│   ├── Participante.txt
│   ├── Evento.txt
│   ├── Instituicao.txt
│   ├── global_id_participante.txt
│   └── ... (outros arquivos de dados)
│
├── Makefile                  # Script de compilação
└── README.md

```
## 👥 Equipe de Desenvolvimento

Este projeto foi desenvolvido colaborativamente com foco na aplicação de conceitos de Engenharia de Software e programação C++.

### 💻 Desenvolvedores Full-Stack

| Membro | Foco de Desenvolvimento | Detalhes da Implementação |
| :--- | :--- | :--- |
| **Gabrielle Santiago Oliveira** | Módulo de Certificados | Lógica de geração e emissão de certificados baseada na participação. |
| **Igor Kramer dos Santos** | Gestão de Entidades | Desenvolvimento das áreas de **Participantes** e **Palestrantes**. |
| **João Pedro da Cunha** | Módulo Institucional | Implementação da área de Instituição, autenticação e configurações. |
| **Jennifer Kalyne Lima Frota** | Operações de Dados | Implementação e otimização das operações **CRUD** e manipulação de registros. |
| **Luan Palma** | **Tech Lead & Full-Stack** | Liderança de equipe, código limpo, arquitetura do sistema e outras adaptações |
| **Pedro Henrique F. Macedo** | Operações de Dados | Implementação e otimização das operações **CRUD** e manipulação de registros. |

## 🙏 Agradecimentos

Gostaríamos de expressar nossa gratidão às instituições e comunidades que tornaram este projeto possível:

* **🏛️ FUCAPI:** Pela base de conhecimentos oferecida no curso, pelo cenário real de estudo de caso e pela valiosa oportunidade de exposição do projeto no **13° Encontro Regional de Engenharia (ENCOENG)**.
* **🌐 Comunidade C++:** Pelo suporte contínuo através de documentações open-source e pela manutenção de um ecossistema robusto que serviu de referência para as boas práticas aplicadas neste projeto.

📄 Licença: Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.
