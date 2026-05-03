# Regras de Workspace: Arquitetura LPaaS, SEO Semântico e GEO (2026)

## 1. Stack Tecnológica e Performance Extrema
- **Framework Opcional:** Astro (prioridade absoluta para arquitetura de ilhas e Zero JavaScript no cliente) ou Next.js 15 (exportação estática e Server Components).
- **Estilização:** Tailwind CSS v4.0. Proibido arquivos CSS externos pesados ou pré-processadores.
- **Métricas Alvo (Core Web Vitals 2026):** O código deve ser otimizado para atingir LCP < 2.0s, INP < 150ms e CLS < 0.05. A latência é inaceitável.

## 2. SEO Semântico e HTML Estrutural
- **Proibido "Div Soup":** O layout deve usar HTML5 semântico rigoroso (`<main>`, `<article>`, `<section>`, `<aside>`, `<nav>`). Isso é crítico para "crawlers cegos" de IA entenderem a hierarquia.
- **Hierarquia de Títulos:** Siga estritamente a ordem H1 -> H2 -> H3. Nunca pule níveis.
- **Imagens:** Use APENAS formatos de próxima geração (WebP/AVIF). Toda imagem deve obrigatoriamente possuir atributo `alt` descritivo focando na intenção e legendas claras para melhorar o parsing de IAs multimodais.

## 3. GEO (Generative Engine Optimization) e Indexação por IA
- **Design "Answer-First" (Answer Hooks):** Formate subtítulos (H2/H3) como perguntas frequentemente feitas pelos usuários. Imediatamente após o título, o primeiro parágrafo DEVE ser uma resposta direta e factual de 40 a 60 palavras, ideal para ser extraída como citação por IAs.
- **Densidade de Fatos (Information Gain):** Evite jargões de marketing vazios ("fluff"). As páginas devem incluir dados, estatísticas reais, casos de estudo ou fontes em blocos de 150-200 palavras.
- **Legibilidade para Máquinas:** Maximize o uso de tabelas HTML/Markdown, listas numeradas e bullet points. Modelos de linguagem (LLMs) priorizam tabelas para comparações e listas para instruções.
- **Arquitetura de Robôs:** Gere automaticamente os arquivos `llms.txt` e `llms-full.txt` na raiz do servidor para servir como mapa estruturado da documentação/site exclusivo para bots de IA (como GPTBot e ClaudeBot).

## 4. Domínio de Entidades e Schema Markup (JSON-LD)
- **Implementação Obrigatória:** Utilize exclusivamente JSON-LD aninhado via `@graph` dentro da tag `<head>`.
- **Entidade Oficial:** A empresa se chama **Anúncio e Site**. Todas as tags `<title>`, `alt` de imagens e metadados gerados devem usar "Anúncio e Site" como autoridade de marca.
- **Identidade da Empresa:** Incorpore os schemas `Organization` ou `LocalBusiness` com o nome "Anúncio e Site". Utilize a propriedade `sameAs` para linkar os perfis da marca no LinkedIn/Wikidata (para desambiguação e verificação) e a propriedade `knowsAbout` para declarar os tópicos de expertise (ex: "SEO", "Desenvolvimento Web", "Landing Pages", "Performance").
- **Tipos de Conteúdo:** Adicione `Article` ou `BlogPosting` em páginas de leitura (usando a propriedade `author` linkada a um schema `Person`). Se houver perguntas, gere um `FAQPage` schema válido.
- **Speakable Schema:** Marque os parágrafos contendo as respostas mais diretas com o schema `Speakable` para captura via assistentes de voz.

## 5. Roteamento Programático e Risco de Conteúdo Duplicado
- **Hub and Spoke:** Construa a estrutura de links internos de forma lógica. As Landing Pages secundárias (Spokes) devem apontar para a página da categoria principal (Hub) e vice-versa usando texto âncora descritivo para facilitar o mapeamento do Knowledge Graph.
- **Canonical Tags:** Todas as variações de Landing Pages do SEO Programático devem receber a tag `<link rel="canonical">` autorreferenciada para assegurar proteção contra penalidades de conteúdo duplicado do Google.
Por que essas regras garantem a vanguarda em 2026?