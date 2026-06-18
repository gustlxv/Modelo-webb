# 🎓 Sistema de Gerenciamento Escolar - Banco de Dados

Este projeto apresenta a modelagem conceitual de um banco de dados para gerenciamento de uma instituição de ensino. O sistema foi desenvolvido para controlar informações de alunos, professores, turmas e disciplinas, permitindo organizar o ambiente acadêmico de forma estruturada e eficiente.

---

## 🎯 Objetivo

O objetivo deste banco de dados é armazenar e gerenciar informações relacionadas ao ambiente escolar, facilitando o controle de:

- Cadastro de alunos;
- Cadastro de professores;
- Controle de turmas;
- Organização das disciplinas;
- Relacionamento entre alunos, professores e turmas.

---

## 🛠️ Modelo Conceitual

O banco de dados foi modelado utilizando o Modelo Entidade-Relacionamento (MER), contendo quatro entidades principais:

### 👨‍🏫 Professor

Armazena os dados dos professores da instituição.

#### Atributos:
- Id_Professor (Chave Primária)
- Nome
- CPF
- Telefone
- Email
- Formação Acadêmica

---

### 👨‍🎓 Aluno

Armazena os dados dos alunos matriculados.

#### Atributos:
- Id_Aluno (Chave Primária)
- Nome
- CPF
- Idade
- Telefone
- Endereço
  - Rua
  - Número
  - Bairro
  - Cidade
  - CEP

---

### 🏫 Turma

Representa as turmas da instituição.

#### Atributos:
- Id_Turma (Chave Primária)
- Sala
- Quantidade de Alunos

---

### 📚 Disciplina

Representa as matérias oferecidas pela escola.

#### Atributos:
- Id_Disciplina (Chave Primária)
- Nome
- Ementa
- Ponto Final

---

## 🔗 Relacionamentos

### Leciona

Relaciona Professor e Turma.

**Regra:**
- Um professor pode lecionar uma ou mais turmas.
- Uma turma deve possuir pelo menos um professor.

---

### Ingressado

Relaciona Aluno e Turma.

**Regra:**
- Uma turma pode possuir vários alunos.
- Um aluno deve estar matriculado em uma turma.

---

### Possui

Relaciona Turma e Disciplina.

**Regra:**
- Uma turma possui uma ou mais disciplinas.
- Uma disciplina pode estar associada a várias turmas.

---

## 📊 Cardinalidades

| Relacionamento | Cardinalidade |
|---------------|--------------|
| Professor → Turma | (1,n) |
| Turma → Professor | (1,n) |
| Aluno → Turma | (1,n) |
| Turma → Aluno | (1,n) |
| Turma → Disciplina | (1,n) |
| Disciplina → Turma | (0,n) |

---

## 💡 Benefícios do Sistema

- Organização das informações acadêmicas.
- Facilidade no gerenciamento de alunos e professores.
- Controle das disciplinas ofertadas.
- Melhor estruturação dos dados escolares.
- Base sólida para desenvolvimento de sistemas de gestão escolar.

---

## 📚 Conceitos Aplicados

- Banco de Dados Relacional
- Modelo Entidade-Relacionamento (MER)
- Entidades
- Atributos
- Relacionamentos
- Cardinalidade
- Chaves Primárias
- Modelagem Conceitual

---

## 👨‍💻 Autor

Projeto desenvolvido para fins acadêmicos, com o objetivo de aplicar conceitos de modelagem de banco de dados em um cenário de gestão escolar.
