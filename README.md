# kiki
# why are we here?

## Abstract

This essay argues that for interaction designers, learning to read code is a distinct and essential skill — even as AI generates it from a sentence. Drawing on my own prototyping practice, I examine code as a design material and the gap between describing an outcome and specifying it precisely enough for a machine. I conclude that programming courses remain relevant because the cognitive habits formed through coding are inseparable from shaping interactive experiences.

**Keywords:** interaction design, code literacy, design materials, AI-assisted design, service design

---

## Introduction

I make interactive things — prototypes that respond to a tap, interfaces that guide someone through a service. I enrolled in this course because at some point every one of those things has to become code, and I have spent too many projects stuck at the boundary between my idea and its realisation. In 2026, a language model can generate that code from a single sentence. So why am I here?

My answer is this: the designer's job is not to write programs but to *read* them — to hold the medium in their hands the way a potter holds clay, knowing its grain, its limits, its tendency to crack. That understanding separates a designer who shapes technology from one who merely requests it.
## Code as Material

Last semester I built a browser-based game using AI to generate the code. It connected to an API for real-time image generation, rendered pixel-art characters in a 3D isometric view, and let the user orbit, pan, and zoom the camera. The AI wrote every line — HTML, CSS, JavaScript, WebGL shaders — and on the surface the result looked polished.

But "looked polished" is not the same as "I understood what I had." Every time a small problem surfaced — a flickering texture, a misaligned sprite, a visible seam between tiles — I could only judge the final output. I would describe the symptom to the AI and it would attempt a fix. But because I could not read the code, the AI had to re-read the entire file before making even a one-line change. Each small fix became a full audit. If I could read the code myself, I could locate the problem in seconds and move on.

When the camera orbit felt sluggish, I could not diagnose why. The code was opaque to me in exactly the way that clay is opaque to someone who has never touched it: you can describe the shape you want, but you cannot feel where it is too thin, where it will collapse in the kiln.

This is why I argue that code is a design material, not merely a delivery mechanism. Wiberg (2018) frames this as part of a broader "material turn" in interaction design — a shift from designing representations of behaviour to designing through the material properties of the medium itself. A material is something whose properties — weight, texture, resistance, failure modes — you learn through direct engagement. Vallgårda et al. (2017) extend this further with "material programming," arguing that designers must engage directly with computational materials to maintain first-hand access to cause-and-effect relationships. You cannot outsource that learning to a tool, because the tool does not share your design intent.
## The Gap Between Description and Specification

The project also surfaced the distance between describing what I wanted and specifying it precisely. When I asked for particle effects, the first output was never right — too fast, too slow, wrong direction. It took more than three rounds to reach something acceptable.

The camera controls were worse. I wanted a slow, weighty orbit. The AI's first attempt was twitchy. I said "slower" — it slowed the rotation but kept the acceleration sharp. I said "smoother" — it added easing but overcorrected, and the camera lagged like moving through water. Worst of all, the AI would sometimes forget our earlier conversation and revert changes we had already agreed on.

This is the gap. Describing an outcome — "slower," "smoother" — is not specifying it. Specification requires knowing which parameter to change and what the side effects will be. Dong et al. (2023) demonstrate that even when multiple AI agents collaborate on code generation, the quality of output depends entirely on the precision of human-provided specifications. Peng et al. (2024) observe a similar pattern: designers who describe intent through natural language prompts produce varied outputs but struggle to converge on precise specifications without directly manipulating the underlying parameters. That knowledge lives in the code, not in the conversation.
## Conclusion

Will this course become obsolete? Not if we understand what it is really teaching. The syntax will change — languages evolve, frameworks rise and fall, and AI will keep absorbing more of the writing. But the habits formed by working closely with code — debugging, reading someone else's logic, thinking in constraints — these are not programming skills. They are *design* skills. They are the difference between holding a material and pointing at it from across the room.

Peng et al. (2025) suggest that the future of design tools lies in composing constraints and prompts through direct, embodied interaction — a practice that still demands the designer's judgment about what the material can and cannot do. I came to this course expecting to learn to write code. What I hope to leave with is the ability to read it, to feel its grain, and to know when the machine has given me something that looks right but is not.

---
## References

Dong, Y., Jiang, X., Jin, Z., & Li, G. (2023). Self-collaboration code generation via ChatGPT. *arXiv*. https://doi.org/10.48550/arXiv.2304.07590

Peng, X., Koch, J., & Mackay, W. E. (2024). DesignPrompt: Using multimodal interaction for design exploration with generative AI. In *Proceedings of the 2024 ACM Conference on Designing Interactive Systems* (pp. 1–14). Association for Computing Machinery. https://doi.org/10.1145/3643834.3661588

Peng, X., Koch, J., & Mackay, W. E. (2025). FusAIn: Composing generative AI visual prompts using pen-based interaction. In *Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems* (Article 874, pp. 1–20). Association for Computing Machinery. https://doi.org/10.1145/3706598.3714027

Vallgårda, A., Boer, L., Tsaknaki, V., & Svanæs, D. (2017). Material programming. *Interactions*, *24*(3), 36–41. https://doi.org/10.1145/3057277

Wiberg, M. (2018). *The materiality of interaction: Notes on the materials of interaction design*. MIT Press. https://doi.org/10.7551/mitpress/10427.001.0001