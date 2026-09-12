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

In autumn 2025 I made a browser-based game in which a language model generated all of the code. The game pulled images from an API in real time, drew pixel-art characters in an isometric three-dimensional view, and let the user orbit, pan and zoom the camera. The model wrote every line — HTML, CSS, JavaScript, WebGL shaders — while my own role shrank to stating requirements and judging the result; the outcome looked polished at a glance.
But looking polished was not the same as understanding what I had. Whenever a small fault appeared — a flickering texture, a sprite shifted by half a pixel, a visible seam between tiles — I could only judge the rendered image. I described the symptom and the model proposed a change, yet I had no basis for deciding whether the change addressed the cause or merely masked it. When the camera orbit felt sluggish, I could not tell whether the bottleneck lay in the frame loop, the texture upload or the projection math, and the problem was never properly resolved. Had I been able to read the code, I could have found the relevant lines directly instead of waiting for a full audit of a file I did not understand.
Code, then, functions here as a design material rather than a mere delivery mechanism. A material is something whose properties — weight, texture, resistance, failure modes — are learned through direct engagement. Wiberg (2018) situates this within the broader "material turn" in interaction design: a shift from designing representations of behaviour toward designing through the material properties of the medium itself. Vallgårda et al. (2017) extend the argument with "material programming", holding that designers must engage directly with computational materials if they are to retain first-hand access to the relation between cause and effect. That access cannot be delegated to a tool: the tool optimises for producing something that looks right given a description, and has no stake in the project's evolving constraints. Code differs from clay in that its resistance is inferential rather than tactile — it fails silently and totally rather than gradually — but it remains something one learns only by pushing against it. This is why the practice I adopted in §4 begins from legibility, not from output.
## The Gap Between Description and Specification

The project also surfaced the distance between describing what I wanted and specifying it precisely. Description names what is wanted; specification names the mechanism that produces it. When I asked for particle effects, the first output was never right — too fast, too slow, wrong direction. It took several rounds to reach something acceptable, and it only converged once I stopped saying "faster" and started naming which parameter controlled the emission rate.
The camera controls were worse. I wanted a slow, weighty orbit. The AI's first attempt was twitchy. I said "slower" — it slowed the rotation but kept the acceleration sharp. I said "smoother" — it added easing but overcorrected, and the camera lagged like moving through water. All three attempts failed because each word named a feeling rather than a parameter. Worst of all, the AI would sometimes forget our earlier conversation and revert changes we had already agreed on. That is not just a limitation of the tool: because the specification lived in the conversation rather than in the code, resetting the conversation erased the specification.
This is the gap. Describing an outcome — "slower," "smoother" — is not specifying it. Specification requires knowing which parameter to change and what the side effects will be. Dong et al. (2023) show that when multiple AI agents collaborate on code generation, output quality is strongly conditioned by the precision of human-provided specifications. Peng et al. (2024) observe a similar pattern: designers who describe intent through natural language prompts produce varied outputs but struggle to converge without directly manipulating the underlying parameters. That knowledge lives in the code, not in the conversation.
## Conclusion

Will this course become obsolete? Not if we understand what it is really teaching. The syntax will change — languages evolve, frameworks rise and fall, and AI will keep absorbing more of the writing. But the habits formed by working closely with code — debugging, reading someone else's logic, thinking in constraints — are not merely programming skills. They are design skills, in the sense that they survive the failure of any particular language: debugging is the recognition of failure modes; reading another's logic is the reconstruction of their intent; thinking in constraints is engaging with the material's properties rather than its grammar. They are the difference between holding a material and pointing at it from across the room.
Peng et al. (2025) suggest that the future of design tools lies in composing constraints and prompts through direct, embodied interaction — a practice that still demands the designer's judgment about what the material can and cannot do. I came to this course expecting to learn to write code. What I hope to leave with is the ability to read it, to feel its grain, and to know when the machine has given me something that looks right but is not.

---
## References

Dong, Y., Jiang, X., Jin, Z., & Li, G. (2023). Self-collaboration code generation via ChatGPT. *arXiv*. https://doi.org/10.48550/arXiv.2304.07590

Peng, X., Koch, J., & Mackay, W. E. (2024). DesignPrompt: Using multimodal interaction for design exploration with generative AI. In *Proceedings of the 2024 ACM Conference on Designing Interactive Systems* (pp. 1–14). Association for Computing Machinery. https://doi.org/10.1145/3643834.3661588

Peng, X., Koch, J., & Mackay, W. E. (2025). FusAIn: Composing generative AI visual prompts using pen-based interaction. In *Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems* (Article 874, pp. 1–20). Association for Computing Machinery. https://doi.org/10.1145/3706598.3714027

Vallgårda, A., Boer, L., Tsaknaki, V., & Svanæs, D. (2017). Material programming. *Interactions*, *24*(3), 36–41. https://doi.org/10.1145/3057277

Wiberg, M. (2018). *The materiality of interaction: Notes on the materials of interaction design*. MIT Press. https://doi.org/10.7551/mitpress/10427.001.0001