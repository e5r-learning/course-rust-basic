# course-rust-basic
Curso sobre o básico da linguagem de programação Rust

https://github.com/rylev/learn-rust-the-hard-way

* Hello World
* Evoluir Hello World para Cargo
* A Função main e o básico da função `fn nome(parametros){ codigo; }`
* A macro println!()
* Variáveis com `let`
* Comentários
* Comentários de documentação e o `cargo doc -> file:///...`
* Tipos de variáveis
* Tipos implícitos `let v1 = 100.0`
* Tipos explícitos `let v1:i32 = 100`
* Constantes
* Redefinição de variáveis `let v1 = 100; let v1 = 100.0f`
* Básico de funções:
  - Chamar função `fn f1(){}; fn main(){ f1(); }`
  - Chamar função com parâmetro
  - Função retornar valor
* Operações aritméticas
* Input e Output básico: `println!`, `io::stdin().read_to_string`
* Um pouco mais sobre números
  - Inteiros, com e sem sinal
  - Ponto flutuante
  - Casas decimais `1_000_000_000_000_000` é melhor que `1000000000000000`
  - Octal, Hexadecimal, Decimal
* Arrays
  - Inicializador `let v1 = ["abc", "def", "ghi"]`,  `let v1:i32[] = [0; 4]`
  - iter()
  - slices
  - for, `for v in 0..v1.len() {}`, `for v in v1.iter() {}`
* Fluxos de controle de decisão
  - If, If Else, If Else If
  - Operadores lógicos
  - Match
* Atribuição condicional
  - If let
* Fluxos de repetição
  - While, Loop
  - For (já visto)
* Argumentos do programa `std::env::args()`, `os::args()`
* Propriedade e empréstimo básico
  - Função recebendo propriedade e retornando reatribuição
  - Função recebendo emprestado
* Mutabilidade
* Tipos personalizados
  - Structs
  - Enum
  - impl
* O básico de orientação a objeto
  - Traint e `impl Trait for Type`
* Os tipos de crates
  - Tipo manual no `Cargo.toml`
  - Cargo build gera `exe, rlib, dll`
  - Tipo ao criar `cargo new --lib`
  - Tipo `exe, main.rs`
  - Tipo `lib, lib.rs`
  - Tipo exe híbrido `main.rs + lib.rs + use mylib::, use crate::`
  - Tipo híbrido com vários exe `bin/exe1.rs, bin/exe2.rs`
  - Tipo híbrido com vários exe no `Cargo.toml` `[[bin]]`
* O básico de módulos
  - Usando módulos com `use x::y`
  - Usando vários do módulo `use x::y::{type1, type2}`
  - Usando vários e si mesmo `use x::y::{self, type1, type2}`
  - Usando `mycrate::` ou `crate::`
  - A hierarquia de arquivos com a hierarquia de módulos
  - Usando `pub` para módulos, funções e tipos, propriedades dos tipos
* O calcanhar de aquiles do Rust, `propriedade`
  - Só o mínimo

## Sugestão de cursos avançados

* Entendendo propriedade de uma vez
* Programação avançada com Rust
  - Programação não segura
  - Programação assíncrona e Future
  - Programação assíncrona com Tokio
  - Concorrênia e Paralelismo
* Programação integrada com FFI
  - Usar códigos estáticos de terceiros
  - Usar códigos dinâmicos de terceiros
  - Exportar código para terceiros (C/C++)
  - Criar módulos para Python, Ruby, NodeJS e PHP
* Programação Web (introdução)
  - Criar clientes HTTP só com Rust
  - Criar servidores HTTP só com Rust
  - Criar microserviço só com Rust
  - Criar microserviço com framework
    - Hyper
    - tower-web
    - Actix-web
  - O problema da autorização
    - User+Password
    - Palavra secreta somente (Token)
    - Token de mercado, OAuth + JWT
* Programação com banco de dados
  - SQLite
  - PostgreSQL
  - MySQL
  - ORM + Diesel + Migrations
  - Async + PoolConnection
* Programação WebAssembly com Rust
