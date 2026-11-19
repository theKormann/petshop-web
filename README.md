# Pet Amigo Petshop - Sistema Web (Fase 1)
**Disciplina:** Fundamentos WEB  
**Curso:** Graduação Online - PUCRS  
**Estudante:** Matheus Kormann  
**Fase:** Fase 1 - Estruturação Semântica em HTML Puro (Sem CSS e Sem JavaScript)

---

## 🌐 Links do Projeto

- **Repositório GitHub:** `https://github.com/theKormann/petshop-web` 
- **Sistema Web em Produção (GitHub Pages):** `https://theKormann.github.io/petshop-web/`

---

## 📋 1. Visão Geral do Projeto

Este projeto consiste no desenvolvimento do front-end da plataforma web para o **Pet Amigo Petshop & Centro de Estética Animal**, um sistema de comércio eletrônico de produtos e serviços para animais de estimação.

Em estrita conformidade com as diretrizes da **Fase 1** da disciplina (conteúdo das **Aulas 1 a 5**):
- O sistema foi construído **exclusivamente com HTML5 semântico puro**;
- Não há qualquer arquivo ou regra de estilização **CSS** ou framework **Bootstrap**;
- Não há códigos ou funções em **JavaScript** (funcionalidade reservada para a Fase 2);
- Foi priorizada a hierarquia correta de marcação, acessibilidade (W3C), navegação intuitiva e estruturação limpa.

---

## 🐾 2. Estrutura do Sistema e Categorias Atendidas

### 2.1. Categorias de Produtos
O catálogo conta com pelo menos 2 produtos em cada uma das 3 categorias obrigatórias (apresentando 3 em cada para maior riqueza de conteúdo):

1. **Acessórios:**
   - *Cama Nuvem Confort Ortopédica (Tam G):* R$ 149,90
   - *Peitoral Antipuxão Ergonômico com Guia (Tam M):* R$ 89,90
   - *Brinquedo Mordedor Interativo Dispenser:* R$ 45,50
2. **Rações Não Perecíveis:**
   - *Ração Seca Super Premium Cães Adultos (15 kg) Frango e Arroz:* R$ 229,90
   - *Ração Seca Premium Especial Gatos Castrados (3 kg) Salmão:* R$ 78,90
   - *Ração Seca Premium Filhotes Todas as Raças (10,1 kg) Carne & Vegetais:* R$ 139,00
3. **Produtos de Higiene e Limpeza:**
   - *Tapete Higiênico Descartável Carvão Ativado (30 un.) 80x60cm:* R$ 69,90
   - *Shampoo Neutro Hipoalergênico & Condicionador 2 em 1 (500 ml):* R$ 34,90
   - *Fraldas Descartáveis Anatômicas Pet (12 un.) Tam M:* R$ 42,90

### 2.2. Serviços do Petshop (Banho e Tosa)
Os serviços contemplam descrição detalhada dos procedimentos, discriminação por porte do animal e apresentação clara das modalidades:
- **Sem Tele-Busca (Balcão):** Tutor traz e retira o animal.
- **Com Tele-Busca (Leva & Traz):** Transporte climatizado em veículo adaptado com caixas individuais em raio de até 10 km.

Valores dos serviços:
- **Banho Completo Tradicional:** R$ 55,00 a R$ 85,00 (sem tele-busca) | R$ 80,00 a R$ 115,00 (com tele-busca).
- **Tosa Higiênica + Banho:** R$ 75,00 a R$ 110,00 (sem tele-busca) | R$ 100,00 a R$ 140,00 (com tele-busca).
- **Tosa Geral da Raça / Máquina + Banho:** R$ 100,00 a R$ 150,00 (sem tele-busca) | R$ 125,00 a R$ 180,00 (com tele-busca).
- **Banho Especial para Felinos:** R$ 80,00 (sem tele-busca) | R$ 105,00 (com tele-busca).

---

## 📂 3. Organização dos Arquivos do Projeto

```text
petshop-web/
├── index.html              # Página inicial com visão geral, produtos e serviços em destaque
├── produtos.html           # Catálogo completo das 3 categorias e tabela consolidada
├── servicos.html           # Descrição dos serviços, tabela com/sem tele-busca e formulário
├── ajuda.html              # Central de ajuda, FAQ, manual de navegação e mapa do site
├── README.md               # Documentação técnica e guia do repositório
└── imagens/                # Imagens vetoriais locais (SVG) sem dependência externa
    ├── logo-petshop.svg
    ├── acessorio-cama-nuvem.svg
    ├── acessorio-peitoral-guia.svg
    ├── acessorio-brinquedo-mordedor.svg
    ├── racao-caes-adultos.svg
    ├── racao-gatos-castrados.svg
    ├── racao-filhotes.svg
    ├── higiene-tapete-higienico.svg
    ├── higiene-shampoo-pet.svg
    ├── higiene-fraldas-pet.svg
    ├── servico-banho-tosa.svg
    └── servico-tele-busca.svg
```

---

## 🛠️ 4. Conceitos das Aulas 1 a 5 Aplicados

- **Aula 1 (Introdução e Estrutura Básica):** Declaração `<!DOCTYPE html>`, estrutura `<html>`, `<head>`, metadados (`charset="UTF-8"`, `viewport`), tags de título e cabeçalho.
- **Aula 2 (Textos e Hierarquia):** Utilização semântica de `<h1>` a `<h4>`, parágrafos `<p>`, divisores `<hr>`, ênfases `<strong>` e `<em>`, endereço `<address>`.
- **Aula 3 (Listas e Hiperlinks):** Menus e listas com `<ul>`, `<ol>`, `<li>`, listas de definição `<dl>`, `<dt>`, `<dd>` para glossário/FAQ, hiperlinks relativos (`<a href="...">`) e links âncora internos.
- **Aula 4 (Mídias e Tabelas):** Imagens semânticas com `<figure>`, `<img>` (atributos `alt`, `width`, `height`) e `<figcaption>`; tabelas ricas (`<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, `<th>` com `scope` e `<td>`).
- **Aula 5 (Semântica Estrutural e Formulários):** Tags semânticas `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`; formulário de agendamento com `<form>`, `<fieldset>`, `<legend>`, `<label for="...">`, `<input>`, `<select>`, `<textarea>` e `<button>`.

---
