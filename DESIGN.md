# Design System: Engenharia de Conversão (Anti-Lovable V1.0)

Este documento define os padrões visuais e técnicos para a interface da agência. O Stitch deve seguir rigorosamente estas definições para garantir uma estética de "Engenharia de Elite" e "High-Performance SaaS".

## 1. Paleta de Cores (Core Palette)
A base é o contraste infinito e a profundidade. Evitar cores saturadas em excesso.

* **Background (Canvas):** `#000000` (Pure Black)
* **Surface (Cards/Bento):** `#09090B` (Zinc-950) com opacidade de 80% (Glassmorphism)
* **Primary Accent:** `#6366F1` (Electric Indigo) - Usar para estados ativos, feixes de luz e CTAs principais.
* **Secondary Accent:** `#10B981` (Emerald) - Usar APENAS para indicadores de "Online", "Sucesso" ou "Performance 100%".
* **Border High:** `#1F2937` (Slate-800)
* **Border Low:** `#111827` (Slate-900)
* **Text Primary:** `#F9FAFB` (Ghost White)
* **Text Secondary:** `#94A3B8` (Slate-400)

## 2. Tipografia (Typography)
O objetivo é clareza técnica e autoridade.

* **Headings (Títulos):** `Geist Sans` ou `Inter`. 
    * *Regra:* Peso Bold (700), Tracking (espaçamento) de `-0.02em`.
* **Body (Corpo):** `Inter`.
    * *Regra:* Peso Regular (400), Line-height de `1.6`.
* **Technical/Metrics:** `JetBrains Mono` ou `Geist Mono`.
    * *Uso:* Números de performance, badges de carregamento, labels de botões técnicos.

## 3. Padrões de Componentes (Component Specs)

### 3.1 Buttons (CTAs)
* **Primary:** Background Indigo (`#6366F1`), Texto Branco. Sem bordas arredondadas exageradas (máximo 8px).
* **Secondary:** Ghost button com borda de 1px Indigo e efeito de hover com brilho sutil (glow).

### 3.2 Bento Grid (Layout)
* Utilizar proporções variadas (1x1, 2x1, 2x2).
* Cada card deve ter uma borda de gradiente linear (`border-image`) que brilha mais intensamente no canto superior esquerdo.
* Background do card com `backdrop-filter: blur(12px)`.

### 3.3 Badges de Performance
* Sempre flutuantes perto de elementos de valor.
* Estilo: Fundo escuro semi-transparente, borda fina Indigo, texto em Monospace.

## 4. Regras de Interface (The "Anti-Lovable" Rules)
1.  **Sem Ilustrações Fofas:** Proibido o uso de personagens 3D ou ilustrações orgânicas. Usar diagramas técnicos, grids e ícones em outline (0.5px).
2.  **Textura de Hardware:** O fundo preto deve ter um ruído (Film Grain) de 2% para evitar gradientes "bandados" e dar aspecto de material físico.
3.  **Grids de Engenharia:** Usar um padrão de pontos (`dotted background`) com opacidade de 5% em seções de transição.
4.  **Velocidade Visual:** Transições devem ser imediatas (máximo 150ms). Nada de animações lentas ou elásticas.

## 5. Copy & Tone
* **Tom:** Direto, técnico, focado em ROI.
* **Palavras-Chave:** Precisão, Código Puro, Latência Zero, Conversão Nativa.

## 6. Brand Identity (Logotype)
* **Nome Oficial:** Anúncio e Site
* **Regra Estrita:** A marca é APENAS tipográfica (Wordmark). Proibido uso de ícones, símbolos ou ilustrações.
* **Tipografia:** Inter ou Geist Sans
* **Peso:** ExtraBold (800)
* **Tracking:** -0.03em
* **Cores:**
  - "Anúncio": Text Primary (#F9FAFB - Ghost White)
  - "Site": Primary Accent (#6366F1 - Electric Indigo)
* **Exemplo:** `<span class="text-text-primary">Anúncio</span><span class="text-[#6366F1]">e Site</span>`
