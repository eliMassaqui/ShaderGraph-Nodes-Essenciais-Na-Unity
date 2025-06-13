# Unity Shader Graph: Guia Prático (Baseado em Daniel Ilett + Livro)

Este guia reúne os nós essenciais usados até a Parte 11 da série *Unity Shader Graph Basics* de Daniel Ilett, complementado com conceitos do livro *Building Quality Shaders for Unity Using Shader Graphs* de Daniel Ilett.

---

## Parte 1 – Introdução ao Shader Graph
> Fundamentos: cor básica, tempo e animações simples.

- **Color**
- **Time**
- **Sine**
- **Multiply**
- **Master Node (URP Lit ou Unlit)**

---

## Parte 2 – Animações com Tempo
> Animações UV e efeitos visuais dinâmicos.

- **Time**
- **Sine**
- **Tiling and Offset**
- **UV**
- **Panner**
- **Sample Texture 2D**

---

## Parte 3 – Transparência e Alpha Clipping
> Criando transparência baseada em máscara ou valor.

- **Alpha Clip Threshold**
- **Split**
- **Step**
- **One Minus**
- **Lerp**
- **Boolean Toggle**

---

## Parte 4 – Fresnel Effect (Borda Brilhante)
> Efeito de brilho nas bordas, útil para objetos mágicos.

- **Fresnel Effect**
- **View Direction**
- **Dot**
- **Normalize**
- **Power**
- **HDR Color**

---

## Parte 5 – Vertex Shaders (Movimento)
> Manipulação de vértices para efeitos de onda ou deformação.

- **Position (Object)**
- **Sine / Cosine**
- **Vector3**
- **Add / Multiply**
- **Set Position**

---

## Parte 6 – Luz e Emissão
> Introdução ao comportamento da luz no shader.

- **Light Direction**
- **Dot Product**
- **Normalize**
- **Color**
- **Emission**

---

## Parte 7 – Iluminação Customizada
> Construção manual de iluminação (sem depender do Lit Master).

- **Custom Lighting Output**
- **Fresnel Effect**
- **Step / Smoothstep**
- **Ambient Light Intensity**
- **Lerp**
- **Add**

---

## Parte 8 – Interseções com Cena (1)
> Detectar onde um objeto toca o chão ou outro objeto.

- **Scene Depth**
- **Screen Position**
- **World Position**
- **Subtract**
- **Compare**
- **Lerp com cor de contato**

---

## Parte 9 – Interseções com Cena (2)
> Aprimorando a técnica de detecção de colisão visual.

- **Depth Fade**
- **Scene Color**
- **Camera Position**
- **Distance**
- **Clamp**
- **Saturate**

---

## Parte 10 – Funções Customizadas
> Importando lógica HLSL dentro do Shader Graph.

- **Custom Function Node**
- **Vector Inputs**
- **HLSL Snippets**
- **Float ou Texture Output**

---

## Parte 11 – Aplicações em Terrain
> Técnicas alternativas para usar Shader Graph com terrenos.

- **Terrain Layer Mapping (manual)**
- **Texture Blending**
- **Splatmap UV**
- **Sample Texture**
- **Height Map (usando Lerp com máscaras)**
- **Normal Map**
- **Triplanar Mapping (opcional)**

---

## Conceitos adicionais (Livro)
> Extras aprendidos no livro não explorados nos vídeos:

- **Fake Lighting (via Ramp Texture)**
- **Dithering Transparency**
- **Texture Atlas e Sprite Sheet**
- **Object Space vs World Space**
- **Dissolve Shader (com Noise e Threshold)**
- **Decal Shader**
- **Edge Detection com Sobel Filter (via Scene Color)**

---

## 📌 Dicas de Fluxo
1. **Sempre normalize vetores** ao trabalhar com direção.
2. **Use `Clamp`, `Saturate` e `Smoothstep`** para evitar valores quebrados.
3. **Combinar UV + Noise + Time** = efeitos incríveis!
4. **Post Processing ativo (Bloom)** ajuda a destacar Emission.

---

## 🔗 Recursos
- YouTube: [Daniel Ilett Channel](https://www.youtube.com/@danielilett)
- Livro: *Building Quality Shaders for Unity Using Shader Graphs*
- Shader Graph Doc: [Unity Manual](https://docs.unity3d.com/Packages/com.unity.shadergraph)

