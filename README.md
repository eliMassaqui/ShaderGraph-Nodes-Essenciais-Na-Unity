# Unity Shader Graph: Guia Prático (Baseado em Daniel Ilett + Livro)

> Repositório com os nós essenciais usados até a Parte 11 da série *Unity Shader Graph Basics* de Daniel Ilett, complementado com técnicas práticas do livro *Building Quality Shaders for Unity Using Shader Graphs*.

---

## Parte 1 – Introdução ao Shader Graph
> Fundamentos: cor básica, tempo e animações simples.

- `Color`
- `Time`
- `Sine`
- `Multiply`
- `Master Node` (`URP Lit` ou `Unlit`)

---

## Parte 2 – Animações com Tempo
> Animações UV e efeitos visuais dinâmicos.

- `Time`
- `Sine`
- `Tiling and Offset`
- `UV`
- `Panner`
- `Sample Texture 2D`

---

## Parte 3 – Transparência e Alpha Clipping
> Criando transparência baseada em máscara ou valor.

- `Alpha Clip Threshold`
- `Split`
- `Step`
- `One Minus`
- `Lerp`
- `Boolean Toggle`

---

## Parte 4 – `Fresnel Effect` (Borda Brilhante)
> Efeito de brilho nas bordas, útil para objetos mágicos.

- `Fresnel Effect`
- `View Direction`
- `Dot`
- `Normalize`
- `Power`
- `HDR Color`

---

## Parte 5 – Vertex Shaders (Movimento)
> Manipulação de vértices para efeitos de onda ou deformação.

- `Position (Object)`
- `Sine` / `Cosine`
- `Vector3`
- `Add` / `Multiply`
- `Set Position`

---

## Parte 6 – Luz e Emissão
> Introdução ao comportamento da luz no shader.

- `Light Direction`
- `Dot Product`
- `Normalize`
- `Color`
- `Emission`

---

## Parte 7 – Iluminação Customizada
> Construção manual de iluminação (sem depender do `Lit Master`).

- `Custom Lighting Output`
- `Fresnel Effect`
- `Step` / `Smoothstep`
- `Ambient Light Intensity`
- `Lerp`
- `Add`

---

## Parte 8 – Interseções com Cena (1)
> Detectar onde um objeto toca o chão ou outro objeto.

- `Scene Depth`
- `Screen Position`
- `World Position`
- `Subtract`
- `Compare`
- `Lerp` (com cor de contato)

---

## Parte 9 – Interseções com Cena (2)
> Aprimorando a técnica de detecção de colisão visual.

- `Depth Fade`
- `Scene Color`
- `Camera Position`
- `Distance`
- `Clamp`
- `Saturate`

---

## Parte 10 – Funções Customizadas
> Importando lógica `HLSL` dentro do Shader Graph.

- `Custom Function`
- `Vector Inputs`
- `HLSL Snippets`
- `Float` ou `Texture Output`

---

## Parte 11 – Aplicações em `Terrain`
> Técnicas alternativas para usar `Shader Graph` com terrenos.

- `Terrain Layer Mapping` (manual)
- `Texture Blending`
- `Splatmap UV`
- `Sample Texture`
- `Height Map` (com `Lerp` e máscaras)
- `Normal Map`
- `Triplanar Mapping` (opcional)

---

## 📘 Conceitos Adicionais (Livro)

> Extras aprendidos no livro **não mostrados nos vídeos**:

- `Fake Lighting` (via `Ramp Texture`)
- `Dithering Transparency`
- `Texture Atlas` e `Sprite Sheet`
- `Object Space` vs `World Space`
- `Dissolve Shader` (com `Noise` e `Threshold`)
- `Decal Shader`
- `Edge Detection` com `Sobel Filter` (via `Scene Color`)

---

## ✅ Tabela Rápida de Aplicações

| 🔧 Node               | 📌 Uso Comum                   | 🧠 Aplicação                  |
|-----------------------|-------------------------------|------------------------------|
| `Lerp`                | Mistura entre valores         | Dissolve, blends, fade       |
| `Fresnel Effect`      | Brilho nas bordas             | Objetos mágicos, destaque    |
| `Depth Fade`          | Suavizar bordas imersas       | Interseção com água, chão    |
| `Custom Function`     | Código HLSL embutido          | Efeitos avançados            |
| `Panner` + `Time`     | Movimento contínuo de textura | Fogo, água, energia          |
| `Alpha Clip Threshold`| Transparência com máscara     | Folhas, grades, vidros       |
| `Scene Depth`         | Profundidade na cena          | Interações físicas visuais   |

---

## 💡 Dicas de Fluxo

1. Sempre use `Normalize` antes de usar `Dot` com vetores.
2. `Clamp`, `Saturate` e `Smoothstep` controlam valores extremos.
3. `Time` + `Noise` = movimento natural.
4. Para brilho forte: use `HDR Color` + `Emission` + pós-processamento `Bloom`.

---

## 🔗 Recursos

- 📺 YouTube: [Daniel Ilett Channel](https://www.youtube.com/@danielilett)
- 📚 Livro: *Building Quality Shaders for Unity Using Shader Graphs*
- 📄 Shader Graph Docs: [Unity Manual](https://docs.unity3d.com/Packages/com.unity.shadergraph)

---

<p align="center">
  <img src="preview-shadergraph.png" width="600" alt="Preview do Shader Graph">
</p>
