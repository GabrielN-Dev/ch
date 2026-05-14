# Churrascaria Grill House - Sistema de Reservas

Este é um projeto de sistema de gestão de reservas para uma churrascaria, desenvolvido como parte do curso técnico em Informática para Internet no **IFSP (Instituto Federal de São Paulo)**. Foi um dos meus primeiros contatos com desenvolvimento Web utilizando PHP e Programação Orientada a Objetos (POO).

## 📌 Sobre o Projeto

O objetivo principal foi criar uma plataforma funcional onde clientes pudessem se cadastrar, realizar login e agendar mesas de forma digital. O projeto foca na lógica de backend, persistência de dados e segurança básica.

## 🚀 Funcionalidades

- **Cadastro de Usuários:** Registro de novos clientes com armazenamento seguro de senhas utilizando `password_hash`.
- **Autenticação:** Sistema de login com verificação de credenciais e gestão de sessões (`session_start`).
- **Reserva de Mesas:** - Reservas diretas para usuários logados.
  - Possibilidade de realizar reservas para terceiros (pessoas sem conta).
- **Segurança:** Uso de *Prepared Statements* (MySQLi) para prevenção de ataques de SQL Injection.
- **Interface Responsiva:** Design simples utilizando HTML5 e CSS3.

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** PHP 7+ (Arquitetura em Classes/POO)
- **Banco de Dados:** MySQL
- **Frontend:** HTML5, CSS3 e JavaScript
- **Servidor Local Recomendado:** XAMPP, WAMP ou Laragon

## 📂 Estrutura de Arquivos Principal

- `conexao.php`: Configuração da conexão com o banco de dados.
- `Usuario.php`: Classe responsável pelo gerenciamento de dados do usuário (Cadastro).
- `Autenticacao.php`: Classe que lida com a lógica de login e verificação de hash.
- `Mesa.php`: Classe para processamento das reservas.
- `reserva_de_mesa_teste.php`: Interface principal para agendamento de mesas.

## 🔧 Como Executar

1. Clone este repositório para a pasta `htdocs` (XAMPP) ou `www` (Laragon).
2. Certifique-se de que o MySQL está rodando.
3. Crie um banco de dados chamado `prj_churrascaria`.
4. Crie as tabelas necessárias (referenciadas nos métodos `INSERT` das classes):
   - `cadastro` (id, nome, telefone, email, senha)
   - `reserva` (id, email_mesa, num_pessoa, dia, horas, mensagem)
5. Acesse `index1.html` pelo seu navegador através do `localhost`.

---
*Este projeto tem fins didáticos e representa o início da minha jornada no desenvolvimento de software.*
