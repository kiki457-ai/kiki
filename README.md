# kiki
# why are we here?

## Abstract

This essay argues that for interaction designers, learning to read code is an essential skill — even as AI generates it from a sentence. Drawing on my prototyping practice, I examine code as a design material and the gap between describing an outcome and specifying it precisely for a machine. I conclude that programming courses stay relevant because the cognitive habits formed through coding are inseparable from shaping interactive experiences.

**Keywords:** interaction design, code literacy, design materials, AI-assisted design, service design

---

## Introduction

I make interactive things — prototypes that respond to a tap, interfaces that guide users through a service. I enrolled in this course because every such project eventually becomes code, and I have spent too many projects stuck between idea and realisation. In 2026, a language model can generate that code from a single sentence. So why am I here?

My answer: the designer's job is not to write programs but to read them — to hold the medium like a potter holds clay, knowing its grain, limits, and tendency to crack. This understanding separates a designer who shapes technology from one who merely requests it.

## Code as Material

In autumn 2025 I made a browser game where a language model generated all code. It pulled images from an API, drew pixel-art in an isometric 3D view, and let users orbit, pan, and zoom. The model wrote every line — HTML, CSS, JavaScript, WebGL shaders — while my role shrank to stating requirements and judging results; it looked polished.

But looking polished differed from understanding it. When faults appeared — flickering textures, sprites shifted by half a pixel, visible seams — I could only judge the rendered image. I described symptoms and the model proposed changes, yet I couldn't tell if they fixed the cause or masked it. When the camera lagged, I couldn't pinpoint the bottleneck — frame loop, texture upload, or projection math — and it was never resolved. Had I read the code, I'd have found the lines directly instead of waiting for an audit of an opaque file.

Code functions as a design material, not a delivery mechanism. Materials have properties — weight, texture, resistance, failure modes — learned through engagement. Wiberg (2018) situates this in the "material turn": shifting from designing representations to designing through material properties. Vallgårda et al. (2017) extend this with "material programming," arguing designers must engage directly with computational materials to retain access to cause and effect. This access can't be delegated: tools optimise for plausible output given a description, with no stake in project constraints. Code differs from clay in that its resistance is inferential rather than tactile — it fails silently and totally — but remains learned only by pushing against it. This is why my practice begins with legibility, not output.

## The Gap Between Description and Specification

The project revealed the gap between describing what I wanted and specifying it. Description names the goal; specification names the mechanism. When I requested particle effects, initial outputs were wrong — too fast, too slow, wrong direction. Convergence required naming the parameter controlling emission rate, not just saying "faster."

Camera controls were worse. I wanted a slow, weighty orbit. The AI's first attempt was twitchy. "Slower" reduced rotation but kept acceleration sharp. "Smoother" added easing but overcorrected, making the camera lag. Each word named a feeling, not a parameter. Worse, the AI sometimes forgot context and reverted agreed changes. Because the specification lived in conversation, not code, resetting it erased the specification.

This is the gap. Describing an outcome is not specifying it. Specification requires knowing which parameter to change and its side effects. Dong et al. (2023) show AI code generation quality depends on specification precision. Peng et al. (2024) observe designers using natural language produce varied outputs but struggle without manipulating parameters. That knowledge lives in code, not conversation.

## Conclusion

Will this course become obsolete? Not if we understand its purpose. Syntax changes — languages evolve, frameworks rise and fall, AI absorbs more writing. But habits from working closely with code — debugging, reading logic, thinking in constraints — are design skills. They survive any language: debugging recognises failure modes; reading logic reconstructs intent; thinking in constraints engages with material properties, not grammar. They separate holding a material from pointing at it.

Peng et al. (2025) suggest future tools will compose constraints and prompts through embodied interaction — still demanding designer judgment about material limits. I came expecting to write code; I hope to leave able to read it, feel its grain, and know when the machine gives something that looks right but is not.
---
## References

Dong, Y., Jiang, X., Jin, Z., & Li, G. (2023). Self-collaboration code generation via ChatGPT. *arXiv*. https://doi.org/10.48550/arXiv.2304.07590

Peng, X., Koch, J., & Mackay, W. E. (2024). DesignPrompt: Using multimodal interaction for design exploration with generative AI. In *Proceedings of the 2024 ACM Conference on Designing Interactive Systems* (pp. 1–14). Association for Computing Machinery. https://doi.org/10.1145/3643834.3661588

Peng, X., Koch, J., & Mackay, W. E. (2025). FusAIn: Composing generative AI visual prompts using pen-based interaction. In *Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems* (Article 874, pp. 1–20). Association for Computing Machinery. https://doi.org/10.1145/3706598.3714027

Vallgårda, A., Boer, L., Tsaknaki, V., & Svanæs, D. (2017). Material programming. *Interactions*, *24*(3), 36–41. https://doi.org/10.1145/3057277

Wiberg, M. (2018). *The materiality of interaction: Notes on the materials of interaction design*. MIT Press. https://doi.org/10.7551/mitpress/10427.001.0001