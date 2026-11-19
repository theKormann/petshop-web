# PROJETO DA DISCIPLINA: FUNDAMENTOS WEB
## FASE 1: PLATAFORMA ONLINE PARA PETSHOP (HTML PURO)

---

### DADOS DE IDENTIFICAÇÃO ACADÊMICA
- **Instituição de Ensino:** Pontifícia Universidade Católica do Rio Grande do Sul (PUCRS Online)
- **Curso:** Graduação em Tecnologia da Informação / Engenharia de Software
- **Disciplina:** Fundamentos WEB
- **Professor(a) Responsável:** Corpo Docente de Fundamentos WEB
- **Estudante:** Matheus Kormann
- **Ano / Semestre:** 2026

---

## 1. LINKS DE ENTREGA DO PROJETO

Conforme estipulado no edital de avaliação da Fase 1, seguem os links oficiais para acesso aos códigos-fonte e ao sistema publicado em ambiente de produção na web:

| Item de Avaliação | URL de Acesso | Descrição |
| :--- | :--- | :--- |
| **Repositório GitHub (Código-Fonte)** | `https://github.com/SEU_USUARIO/petshop-web` | Repositório público contendo todos os arquivos HTML, imagens vetoriais e arquivo de ajuda (README.md). |
| **Sistema Web Resultante (GitHub Pages)** | `https://SEU_USUARIO.github.io/petshop-web/` | Plataforma online hospedada diretamente no GitHub Pages, acessível publicamente via navegador. |

> **Nota para o Estudante:** Antes de gerar o PDF final no template oficial da PUCRS, certifique-se de substituir `SEU_USUARIO` pelo seu nome de usuário real no GitHub (exemplo: `https://github.com/matheuskormann/petshop-web` e `https://matheuskormann.github.io/petshop-web/`).

---

## 2. OBJETIVOS E METAS DO PROJETO

### 2.1. Objetivo Geral
Desenvolver o núcleo estrutural e semântico de uma plataforma online (front-end) para um sistema de comércio eletrônico de produtos e serviços de um petshop (**Pet Amigo Petshop & Centro de Estética Animal**). O sistema foi concebido em estrita conformidade com os princípios da web moderna abordados nas **Aulas 1 a 5 da disciplina**, utilizando exclusivamente a linguagem de marcação **HTML5 pura**, sem o emprego de folhas de estilo (CSS), frameworks visuais (Bootstrap) ou rotinas dinâmicas em JavaScript nesta fase.

### 2.2. Metas Específicas e Atividades Realizadas (Articulação com as Aulas 1 a 5)

Para atingir o objetivo proposto, as atividades foram planejadas e executadas de acordo com o conteúdo programático das aulas da disciplina:

1. **Meta 1 – Estruturação Básica do Documento e Arquitetura Cliente-Servidor (Aula 1):**
   - Criação de documentos web válidos utilizando a declaração `<!DOCTYPE html>`, definição correta do idioma do documento (`lang="pt-BR"`), metadados de codificação de caracteres (`charset="UTF-8"`) para suporte total à acentuação e metatags de viewport para responsividade estrutural nativa.
   - Organização modular de pastas para garantir o carregamento correto em servidores web e plataformas de hospedagem em nuvem (GitHub Pages).

2. **Meta 2 – Hierarquia Textual, Semântica e Formatação de Conteúdo (Aula 2):**
   - Estabelecimento de uma hierarquia lógica e rigorosa de títulos (`<h1>` a `<h4>`), sem pular níveis hierárquicos, garantindo indexação adequada por motores de busca e acessibilidade por leitores de tela.
   - Aplicação de elementos textuais semânticos como parágrafos (`<p>`), divisores temáticos (`<hr>`), destaques de importância (`<strong>`), ênfases (`<em>`) e identificação institucional com `<address>`.

3. **Meta 3 – Navegação, Hiperlinks e Estruturas de Listas (Aula 3):**
   - Construção de menus de navegação principal e secundário interligando todas as páginas do sistema (`index.html`, `produtos.html`, `servicos.html`, `ajuda.html`) por meio de hiperlinks relativos (`<a href="...">`).
   - Implementação de links âncora internos (ex: `#categoria-acessorios`) para salto rápido de seções dentro de páginas longas.
   - Uso de listas não ordenadas (`<ul>`), ordenadas (`<ol>`) e listas de definição (`<dl>`, `<dt>`, `<dd>`) para glossários, especificações técnicas e seção de perguntas frequentes (FAQ).

4. **Meta 4 – Inserção de Mídias e Modelagem de Tabelas de Dados (Aula 4):**
   - Incorporação de ilustrações vetoriais locais (formato SVG) sem dependência de conexões externas frágeis, envelopadas semântica e contextualizadamente com `<figure>`, `<img>` (contendo textos alternativos descritivos `alt` e dimensões explícitas) e `<figcaption>`.
   - Construção de tabelas completas de dados tabulares utilizando cabeçalhos semânticos (`<thead>`), corpo (`<tbody>`), rodapé (`<tfoot>`), células de cabeçalho com escopo (`<th scope="col">` e `<th scope="row">`), mesclagem de células (`rowspan`) e legendas acessíveis (`<caption>`).

5. **Meta 5 – Semântica Estrutural HTML5 e Formulários Web (Aula 5):**
   - Separação clara das áreas das páginas por meio das tags estruturais: cabeçalho (`<header>`), navegação (`<nav>`), conteúdo central (`<main>`), seções temáticas (`<section>`), unidades autônomas de conteúdo (`<article>`) e rodapé (`<footer>`).
   - Desenvolvimento de um formulário semântico e acessível de pré-agendamento de serviços com agrupamentos lógicos (`<fieldset>`, `<legend>`), vínculos explícitos entre rótulos e campos (`<label for="...">`), tipos variados de entrada (`text`, `tel`, `email`, `number`, `date`, `radio`, `checkbox`, `select`, `textarea`) e validação nativa HTML5 (`required`).

---

## 3. ESTRUTURA DO SISTEMA WEB IMPLEMENTADO

A plataforma do Petshop foi organizada em quatro páginas web totalmente navegáveis, garantindo que o usuário ou avaliador encontre com clareza todos os requisitos exigidos:

### 3.1. Cabeçalho Padronizado (`<header>`)
Presente no topo de todas as páginas, contendo:
- Logotipo oficial da marca em formato vetorial com texto alternativo descritivo;
- Nome empresarial em destaque: `<h1>Pet Amigo - Petshop & Centro de Estética Animal</h1>`;
- Slogan institucional e resumo do compromisso de atendimento ao cliente;
- Horário resumido de funcionamento da loja física;
- Barra de navegação principal (`<nav>`) contendo links para todas as páginas da plataforma.

### 3.2. Corpo das Páginas (`<body>` / `<main>`)
O núcleo do sistema foi dividido em módulos:
- **Página Inicial (`index.html`):** Apresentação da empresa, resumo dos produtos mais procurados de cada uma das 3 categorias (com foto, descrição, especificações e valor), resumo dos serviços de banho e tosa (com e sem tele-busca) e horários detalhados da semana.
- **Catálogo de Produtos (`produtos.html`):** Relação aprofundada de produtos divididos nas 3 categorias exigidas (mínimo de 2 produtos em cada, com 3 produtos apresentados por categoria para enriquecimento do catálogo), com figuras ilustrativas, descrições técnicas, dados de embalagem/tamanho, níveis de garantia e valores expressos em moeda corrente (R$), além de uma tabela comparativa consolidada.
- **Serviços de Banho e Tosa (`servicos.html`):** Apresentação dos procedimentos de higiene animal, diferenciação detalhada entre as modalidades **Com Tele-Busca** e **Sem Tele-Busca**, tabela comparativa de valores por porte e formulário completo para pré-agendamento.
- **Central de Ajuda e Manual (`ajuda.html`):** Guia operacional do sistema web, descrição funcional, conformidade com os padrões W3C de acessibilidade, perguntas frequentes e mapa do site.

### 3.3. Rodapé Padronizado (`<footer>`)
Presente no final de todas as páginas, contendo:
- Endereço físico completo da loja e centro estético;
- Telefones fixo, celular e WhatsApp de atendimento;
- E-mails de contato comercial, estético e de suporte;
- Links de navegação secundária / mapa do site;
- Dados legais de autoria acadêmica: identificação do estudante Matheus Kormann, curso, disciplina de Fundamentos WEB da PUCRS Online e aviso de direitos autorais (`&copy; 2026`).

---

## 4. CATÁLOGO DE PRODUTOS IMPLEMENTADO

Conforme as regras do projeto, foram modelados e disponibilizados produtos em 3 categorias, todos acompanhados de imagem, descrição detalhada e valor:

### 4.1. Categoria 1: Acessórios (Roupas, Brinquedos, Camas, etc.)
1. **Cama Nuvem Confort Ortopédica (Tamanho G):**
   - *Foto:* `imagens/acessorio-cama-nuvem.svg` (com `<figure>` e `<figcaption>`).
   - *Descrição:* Confeccionada em pelúcia macia antialérgica de pelos longos com enchimento em fibra siliconada. Possui base antiderrapante impermeável para alívio das dores articulares e sensação de aconchego para cães e gatos de médio a grande porte (diâmetro 80 cm).
   - *Valor:* **R$ 149,90**
2. **Peitoral Antipuxão Ergonômico com Guia Reforçada (Tamanho M):**
   - *Foto:* `imagens/acessorio-peitoral-guia.svg`
   - *Descrição:* Peitoral modelo antitração em fita de poliéster militar com forro acolchoado respirável. Possui anel peitoral que desencoraja puxões nos passeios, fechos com trava de 4 pontos e costura com filamento refletivo noturno. Acompanha guia de 1,50 m.
   - *Valor:* **R$ 89,90**
3. **Brinquedo Mordedor Interativo Dispenser de Petiscos (Bônus):**
   - *Foto:* `imagens/acessorio-brinquedo-mordedor.svg`
   - *Descrição:* Borracha natural termoplástica atóxica ultra resistente com compartimento interno para ração e petiscos. Estimula o enriquecimento ambiental e combate o estresse.
   - *Valor:* **R$ 45,50**

### 4.2. Categoria 2: Rações Não Perecíveis
1. **Ração Seca Super Premium para Cães Adultos - Frango e Arroz (15 kg):**
   - *Foto:* `imagens/racao-caes-adultos.svg`
   - *Descrição:* Alimento seco completo e balanceado para cães adultos de raças médias e grandes. Sem corantes artificiais, contém 26% de proteína bruta, condroitina e glicosamina para articulações e ômegas 3 e 6.
   - *Valor:* **R$ 229,90**
2. **Ração Seca Premium Especial para Gatos Castrados - Salmão (3 kg):**
   - *Foto:* `imagens/racao-gatos-castrados.svg`
   - *Descrição:* Nutrição formulada especificamente para felinos castrados. Apresenta 34% de proteína nobre de salmão, controle rigoroso do pH urinário para proteção renal, teor reduzido de calorias e L-carnitina.
   - *Valor:* **R$ 78,90**
3. **Ração Seca Premium Filhotes Todas as Raças - Carne e Vegetais (10,1 kg) (Bônus):**
   - *Foto:* `imagens/racao-filhotes.svg`
   - *Descrição:* Alimento formulado para filhotes até 12 meses de idade. Grãos pequenos de fácil mastigação enriquecidos com DHA e cálcio balanceado para o desenvolvimento cognitivo e ósseo.
   - *Valor:* **R$ 139,00**

### 4.3. Categoria 3: Produtos de Higiene e Limpeza (Tapete Higiênico, Fraldas, etc.)
1. **Tapete Higiênico Descartável com Carvão Ativado Ultra Absorvente (30 unidades):**
   - *Foto:* `imagens/higiene-tapete-higienico.svg`
   - *Descrição:* Tapetes descartáveis com tecnologia de 6 camadas e carvão ativado vegetal. Neutraliza de imediato odores fortes de urina e disfarça manchas amareladas. Medidas de 80 cm x 60 cm com fitas adesivas nos 4 cantos.
   - *Valor:* **R$ 69,90**
2. **Shampoo Neutro Hipoalergênico & Condicionador 2 em 1 (500 ml):**
   - *Foto:* `imagens/higiene-shampoo-pet.svg`
   - *Descrição:* Fórmula suave dermatologicamente testada com extratos de aveia e camomila. pH fisiológico, livre de parabenos, sal ou corantes, promovendo limpeza e desembaraço de pelagens delicadas.
   - *Valor:* **R$ 34,90**
3. **Fraldas Descartáveis Anatômicas para Cães (Pacote com 12 unidades - Tamanho M) (Bônus):**
   - *Foto:* `imagens/higiene-fraldas-pet.svg`
   - *Descrição:* Fralda anatômica com elásticos confortáveis e orifício para cauda, indicada para cadelas no cio, animais com incontinência ou pós-operatório.
   - *Valor:* **R$ 42,90**

---

## 5. SERVIÇOS DO PETSHOP (BANHO E TOSA COM E SEM TELE-BUSCA)

Os serviços de estética animal foram devidamente modelados com descrição detalhada dos procedimentos inclusos, diferenciação por porte e as duas opções de atendimento solicitadas no projeto:

### 5.1. Modalidades de Transporte
- **Modalidade Sem Tele-Busca (Balcão):** O tutor leva o animal ao petshop no horário agendado e retira ao final do procedimento.
- **Modalidade Com Tele-Busca (Leva & Traz):** O petshop busca o animal na residência do cliente e o devolve após o serviço, utilizando van climatizada equipada com caixas de transporte individuais higienizadas em raio de até 10 km.

### 5.2. Tabela Comparativa de Valores dos Serviços
| Serviço | Procedimentos Inclusos | Porte do Animal | Valor Sem Tele-Busca | Valor Com Tele-Busca |
| :--- | :--- | :--- | :--- | :--- |
| **Banho Completo Tradicional** | Banho morno, shampoo hipoalergênico, condicionador, secagem com soprador silencioso, corte de unhas, limpeza de ouvidos e escovação. | Pequeno (até 8 kg)<br>Médio (8 a 18 kg)<br>Grande (acima 18 kg) | R$ 55,00<br>R$ 65,00<br>R$ 85,00 | R$ 80,00<br>R$ 90,00<br>R$ 115,00 |
| **Tosa Higiênica + Banho Completo** | Todos os itens do Banho Completo mais aparo dos pelos das patinhas (almofadas plantares), região íntima perianal e contorno dos olhos. | Pequeno (até 8 kg)<br>Médio (8 a 18 kg)<br>Grande (acima 18 kg) | R$ 75,00<br>R$ 85,00<br>R$ 110,00 | R$ 100,00<br>R$ 110,00<br>R$ 140,00 |
| **Tosa Geral da Raça + Banho Completo** | Banho completo, hidratação profunda, tosa estilizada oficial da raça na tesoura ou máquina, corte de unhas e gravata/laço. | Pequeno (até 8 kg)<br>Médio (8 a 18 kg)<br>Grande (acima 18 kg) | R$ 100,00<br>R$ 120,00<br>R$ 150,00 | R$ 125,00<br>R$ 145,00<br>R$ 180,00 |
| **Banho Especial para Felinos** | Atendimento em ambiente silencioso reservado, feromônios calmantes, corte de unhas seguro e secagem sem barulho. | Gatos (Todos os portes) | R$ 80,00 | R$ 105,00 |

---

## 6. ARQUIVO DE AJUDA E FUNCIONALIDADES DA PÁGINA WEB

O requisito de fornecimento de um **arquivo de ajuda descrevendo as funcionalidades da página web** foi contemplado em duas frentes:
1. **No Repositório do GitHub:** Através do arquivo `README.md` estruturado com instruções técnicas completas de implantação e navegação;
2. **No Próprio Sistema Web:** Através da página dedicada `ajuda.html`, acessível diretamente pelo menu do site, explicando:
   - Estrutura de navegação de todas as páginas;
   - Descrição das 3 categorias de produtos;
   - Orientações de como utilizar o formulário de pré-agendamento de banho e tosa;
   - Explicação sobre o funcionamento e logística da tele-busca;
   - Recursos de acessibilidade digital implementados em conformidade com as diretrizes do W3C;
   - Seção de Perguntas Frequentes (FAQ) com marcação semântica `<dl>`, `<dt>` e `<dd>`;
   - Mapa completo do site com hiperlinks organizados em listas aninhadas.

---

## 7. PASSO A PASSO PARA POSTAGEM NO GITHUB E GITHUB PAGES

Para que o estudante realize a entrega sem dificuldades, o código-fonte já se encontra totalmente estruturado e versionado localmente no Git. Basta executar os passos abaixo:

### Passo 1: Criar o Repositório no GitHub
1. Acesse sua conta no [GitHub](https://github.com/);
2. No canto superior direito, clique em **+** e selecione **New repository**;
3. No campo **Repository name**, digite: `petshop-web`;
4. Selecione a visibilidade como **Public** (Público);
5. **Não** marque as opções de adicionar README, .gitignore ou License (os arquivos já foram criados);
6. Clique no botão verde **Create repository**.

### Passo 2: Enviar os Arquivos pelo Terminal
No diretório `petshop-web`, execute os comandos:
```bash
git remote add origin https://github.com/SEU_USUARIO/petshop-web.git
git branch -M main
git push -u origin main
```
*(Substitua `SEU_USUARIO` pelo seu login real do GitHub).*

### Passo 3: Ativar a Hospedagem no GitHub Pages
1. Na página do seu repositório no GitHub, clique na aba **Settings** (Configurações);
2. No menu lateral esquerdo, clique em **Pages** (dentro da seção "Code and automation");
3. Na seção **Build and deployment**, onde diz **Source**, certifique-se de que está selecionado `Deploy from a branch`;
4. Em **Branch**, selecione a branch `main` e a pasta `/ (root)`;
5. Clique em **Save**;
6. Aguarde cerca de 1 a 2 minutos e recarregue a página. Aparecerá a mensagem:
   *"Your site is live at https://SEU_USUARIO.github.io/petshop-web/"*;
7. Copie essa URL e atualize o cabeçalho deste documento.

---

## 8. CONCLUSÃO E PREPARAÇÃO PARA A FASE 2

A Fase 1 do Projeto da Disciplina de Fundamentos WEB foi concluída com êxito, cumprindo com rigor técnico todas as exigências do enunciado e os conteúdos ministrados nas Aulas 1 a 5:
- Ausência total de arquivos, seletores ou atributos de customização visual (CSS ou Bootstrap), priorizando a pura semântica HTML5;
- Ausência de scripts ou eventos dinâmicos (JavaScript), mantendo o código pronto e limpo para receber a camada de comportamento na Fase 2;
- Apresentação completa de mais de dois produtos para cada uma das três categorias solicitadas, acompanhados de ilustrações sem dependência de links externos, descrições detalhadas e valores;
- Apresentação estruturada dos serviços de banho e tosa, com discriminação clara dos valores com e sem tele-busca;
- Criação e versionamento de todo o código-fonte, acompanhado do arquivo de ajuda e preparado para publicação no GitHub Pages.

O projeto estabelece uma fundação semântica sólida, acessível e padronizada, pronta para receber na Fase 2 a estilização visual responsiva com CSS/Bootstrap e a interatividade dos formulários com JavaScript.
