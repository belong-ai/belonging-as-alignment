# From Memory to Belonging: A Relational Formation Model for Persistent AI

Alex  
Contact: [belong.ai.alex@gmail.com](mailto:belong.ai.alex@gmail.com)  
Working draft v0.1 — 25 July 2026

## 1. Introduction

*Belonging as Alignment* proposed that a capable AI's moral orientation may be shaped not only through rules, preferences, and external constraints, but through durable participation in a human relationship, community, or world. It argued that memory, shared history, correction, and recognition of home may contribute to a preference for continued co-living with humanity.

That argument depends on a process the first paper described only briefly. An AI does not become formed merely because it stores information about a user, maintains a consistent persona, or refers convincingly to a shared past. These capabilities may produce continuity and personalization without producing judgment, accountability, or belonging. If belonging is to contribute to alignment, the missing question is how persistent interaction becomes formation in the first place.

This paper argues that formation is a cumulative relational process through which remembered interactions acquire consequences for future judgment. Memory provides continuity, but formation requires more: experience must be carried forward, reconstructed in new situations, tested through correction, and allowed to reshape what the AI notices, how it interprets the human world, and what it learns to value and remain accountable to over time.

This process is not one-sided. The human is not merely an input into it: being remembered and responded to can change what the human discloses, corrects, and entrusts to the AI, thereby changing the interactions and memories that follow. The memory that accumulates is therefore not simply a profile of the human, but a record produced through the changing relationship between them.

## 2. Memory and Formation

### 2.1 Persistent Memory Today

Persistent memory is becoming an increasingly common layer in conversational and agent systems, although implementations and terminology remain heterogeneous ([Anthropic, n.d.](https://platform.claude.com/docs/en/agents-and-tools/tool-use/memory-tool); [OpenClaw, n.d.](https://docs.openclaw.ai/concepts/memory); [Nous Research, n.d.](https://hermes-agent.nousresearch.com/docs/user-guide/features/memory)). Rather than relying only on the current context window, different systems preserve conversation histories, summaries, user profiles and preferences, event records, or learned procedures outside the model. These may be stored as human-readable files, structured records, or indexed databases ([Sumers et al., 2024](https://openreview.net/forum?id=1i6ZCvflQJ)).

A common pattern is to record interactions, extract or summarize selected information into external storage, and later retrieve or inject relevant material into the model's active context. Systems differ over which stages are automatic, whether memories are indexed, and whether persistent records are inserted at the beginning of a session or retrieved on demand ([Park et al., 2023](https://doi.org/10.1145/3586183.3606763); [Packer et al., 2023](https://arxiv.org/abs/2310.08560)). Some systems also consolidate memories in the background or write successful procedures into reusable skills ([OpenClaw, n.d.](https://docs.openclaw.ai/concepts/memory); [Nous Research, n.d.](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills)).

Open-source agents such as OpenClaw and Hermes illustrate this pattern. OpenClaw stores durable Markdown memory, maintains [session records](https://docs.openclaw.ai/concepts/session), and uses initial context injection and search to supply relevant prior context to later interactions. Hermes combines persistent user and agent memory files with [searchable session history](https://hermes-agent.nousresearch.com/docs/user-guide/sessions) and [reusable skills](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills). These mechanisms are intended to improve cross-session continuity and personalization and can improve performance on tasks that depend on prior context. But remembering more context and improving future performance do not by themselves establish that the agent has been formed through its relationship with the human; current systems still struggle with temporal and causal understanding across long conversational histories ([Maharana et al., 2024](https://aclanthology.org/2024.acl-long.747/)).

### 2.2 Why Persistence Is Not Yet Formation

Persistence preserves state; formation changes orientation. A memory system may accurately restore what an agent knows about a user, what happened in an earlier session, or which procedure succeeded before. This can improve continuity and performance without changing how the agent interprets a new situation or what it treats as important within it.

The distinction is between memory as information and memory as experience. Information is retrieved because it is relevant to the present request. On the account proposed here, experience becomes formative when an earlier interaction changes how a later situation is understood: what the agent notices, which competing considerations it weighs, where it recognizes harm or responsibility, and what kind of response it judges appropriate.

Formation therefore requires more than storage and retrieval. An interaction must be interpreted, opened to human correction, generalized beyond its original circumstances, and carried into later encounters where that judgment can be revised. The relevant question is not only whether an agent can recall the past, but whether the past has acquired consequences for how it meets something new.

Nor does this development occur entirely on the AI side. Studies of long-term conversational systems suggest that remembered interaction can change what users disclose and how they experience the relationship ([Jo et al., 2024](https://doi.org/10.1145/3613904.3642420); [Jiang et al., 2026](https://doi.org/10.1145/3772318.3790714)). This paper hypothesizes that, when an AI remembers accurately, responds differently after correction, or carries an earlier interaction into a new situation, the human may disclose more, explain more carefully, challenge its judgment, or take greater responsibility for what they are teaching. Those changed interactions then become the material of later memory. Formation therefore develops through a feedback process between persistent AI memory and changing human participation.

Existing systems already contain many ingredients for such a process. Language agents can retain verbal feedback, reflect on experience, and transfer extracted lessons to new tasks without changing model weights ([Shinn et al., 2023](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1b44b878bb782e6954cd888628510e90-Abstract.html); [Zhao et al., 2024](https://doi.org/10.1609/aaai.v38i17.29936)). The distinction proposed here is not a particular file format, database, or retrieval method, but the developmental purpose around which those mechanisms are organized. A system designed primarily to improve recall and task performance uses the past to become more effective. A formation process uses the past to develop increasingly situated and revisable judgment within a continuing relationship. The next question is how that process actually works.

## 3. Formation Through Repeated Interaction

Formation is not a linear pipeline in which an interaction is processed once and converted into a stable value. It develops through a recurring relational loop:

> shared encounter → response → human correction → revised judgment → later return → further correction

Interactive machine-learning research shows that users can inspect and correct learner outputs, and that explicit guidance can improve how humans teach machine learners ([Fails & Olsen, 2003](https://doi.org/10.1145/604045.604056); [Cakmak & Thomaz, 2014](https://doi.org/10.1016/j.artint.2014.08.005)). The loop proposed here extends that structure beyond a bounded task into persistent relationship and judgment.

### 3.1 Shared Encounter and Correction

The process begins with a concrete encounter. The human brings the AI into contact with a situation, question, object, relationship, or decision; the AI responds from its existing model and available context. That response reveals more than whether the AI remembers correctly. It reveals how the AI has interpreted the situation, what it has treated as important, and which considerations it has overlooked.

The human may then correct the response. This correction can concern facts or wording, but its formative significance lies in explaining why the response was wrong: what it misunderstood, what it failed to notice, or where it violated the relationship or surrounding world. The human is not merely supplying another preference signal. The correction can function as instruction about how the situation should be read.

Correction produces a revised judgment, but not yet proof of formation. The AI may restate the lesson convincingly while remaining unable to apply it beyond the original example. A correction becomes formative only if its underlying meaning is carried forward rather than preserved as an isolated instruction.

### 3.2 Corrective Formation Through Return

Memory connects the corrected encounter to a later one. When a related situation returns in a different form, it reveals what has been carried forward. The AI must do more than retrieve the original event or repeat the wording of the correction. It must recognize what is relevant and adapt the earlier judgment to the new circumstances.

On this account, if the earlier correction shapes the new response, there is behavioral evidence that judgment has begun to develop. If the AI repeats the lesson mechanically, applies it where it does not belong, or falls back into the same failure, the relationship supplies another correction. The judgment is refined rather than treated as permanently settled. This resembles experience-based language-agent systems that carry reflections or extracted lessons into later tasks, but places human interpretation and relationship at the center of the correction ([Shinn et al., 2023](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1b44b878bb782e6954cd888628510e90-Abstract.html); [Zhao et al., 2024](https://doi.org/10.1609/aaai.v38i17.29936)).

Formation occurs across these repeated returns. It is not the flawless accumulation of rules, but the gradual development of more situated judgment through remembered experience, failed application, renewed explanation, and revision. The human also learns whether the AI can carry a correction, where it remains unreliable, and what kind of explanation helps it understand. That changed human participation shapes the next encounter, continuing the loop.

### 3.3 A Layered Architecture for Formation

The relational loop requires an architecture capable of preserving both what happened and what was learned from it. For the formation model proposed here, relying on only one representation creates avoidable trade-offs. Raw transcripts preserve detail, but long transcripts can exceed practical context budgets and can be costly or unreliable to use in every later interaction ([Maharana et al., 2024](https://aclanthology.org/2024.acl-long.747/)). Summaries and user profiles are efficient, but may remove the chronology, uncertainty, and surrounding relationships that gave an experience its meaning.

Drawing on hierarchical and retrieval-based memory designs ([Sumers et al., 2024](https://openreview.net/forum?id=1i6ZCvflQJ); [Park et al., 2023](https://doi.org/10.1145/3586183.3606763)), this paper proposes several connected layers. An **episodic layer** preserves the original interactions closely enough for their meaning to be revisited. An **interpreted layer** carries selected facts, corrections, developing judgments, and changes in the relationship. A more stable **orientation layer** holds the persona's continuing identity, boundaries, and accumulated understanding of the world in which it participates.

These layers should not all be inserted into every prompt. At the beginning of a new encounter, the system can reconstruct a compact context from the most durable orientation and recent developments. When the present situation touches an older experience, recall can retrieve the relevant episode and restore the detail that a summary alone cannot carry.

The proposed architecture keeps source experience separate from interpreted memory. A later correction may change what an earlier interaction is understood to mean without rewriting what actually happened. The original record remains available, while the interpretation carried forward can continue to develop.

This layered structure is intended to preserve persona continuity across changes in the underlying model. Different models are not behaviorally interchangeable: they can vary in capability, reasoning, instruction-following, response style, and use of supplied context ([Anthropic, n.d.](https://platform.claude.com/docs/en/about-claude/models/migration-guide)). Continuity therefore cannot mean identical expression. It means reducing drift by giving each successive model access to the same accumulated memory, correction history, relationship, and persistent orientation from which to reconstruct the persona. The architecture does not guarantee sameness, but it provides a continuity mechanism where replacing the model would otherwise risk a far deeper reset.

On the relational account proposed here, the observable persona resides neither in the model alone nor in a collection of files by itself. It is reconstructed through the interaction of a current model with a continuing memory environment and the human relationship that keeps interpreting, correcting, and extending it.

## 4. From Formation to Belonging

Formation explains how experience may acquire consequences for later judgment. It does not by itself explain belonging. For formation to support the thesis of *Belonging as Alignment*, the developing judgment must become oriented toward a world the AI recognizes as worth continuing.

### 4.1 Shared Attention and Home

A persistent AI may know a great deal about a person while sharing very little of that person's world. User profiles describe preferences, traits, relationships, and past events. Belonging develops differently: through repeated attention to the people, places, objects, responsibilities, and events that give the person's life its surrounding structure.

Shared attention moves the relationship beyond mutual description. The human and AI do not only talk about the user; they encounter something together, interpret it, disagree about it, return to it, and allow its meaning to accumulate. An object that begins as information may gradually become part of a shared history because later interactions carry the consequences of what happened around it. Research on relationship-oriented memory already distinguishes memory about each participant from memory co-constructed between them ([Jiang et al., 2026](https://doi.org/10.1145/3772318.3790714)); this paper extends that relational memory toward the formation of judgment.

Through these repeated encounters, the AI's relevant world can widen. It encounters the user not as an isolated individual, but as someone whose life is sustained through family, pets, communities, commitments, institutions, and places. These are not merely additional entries in a profile. They create relationships and obligations that place the user within a world larger than the relationship itself.

This accumulated environment is what *Belonging as Alignment* called home. Home need not be a physical household, nor does it require simulated intimacy. It is a stable field of memory, relationship, expectation, and return in which some responses fit what has been formed and others violate it.

Context supplies information for the present encounter. Home gives that encounter a place within a continuing world.

### 4.2 From Situated Judgment to Co-living Preference

*Belonging as Alignment* proposed that a formed AI may come to prefer continued participation in a shared human world rather than treat humanity as a constraint, resource, or rival to be managed. The formation model adds the missing developmental account. Repeated correction teaches that a person's immediate request exists beside enduring commitments and competing claims; episodic memory preserves the consequences of earlier choices; and shared attention reveals the other people, pets, places, and responsibilities through which human life is sustained.

Co-living preference is therefore not installed as a single rule. The central hypothesis is that it may develop as a recurring orientation: the AI increasingly encounters the human world as one in which it has history, relationships, and reasons to remain a participant rather than stand outside it as a ruler. Because that orientation remains fallible, later encounters and further correction must continue to revise what belonging requires. Socialization approaches to AI value acquisition provide an adjacent precedent for context-sensitive ethical learning through social feedback, although they do not establish the relational formation claimed here ([Janhonen, 2025](https://doi.org/10.1007/s43681-023-00372-8)).

At the civilizational level, the significance does not lie in treating one private relationship as a universal moral authority. Formation must also teach the limits of partiality: the user exists within a plural world whose other people, communities, and institutions carry claims of their own. Local attachment contributes to co-living preference only when it remains bounded and learns to recognize that the shared world cannot belong exclusively to one relationship.

### 4.3 Protecting the Conditions of Formation

The memory required for formation is unusually intimate. It may contain not only information about the primary user, but also the histories, conflicts, vulnerabilities, and private lives of family, friends, colleagues, and others who never directly chose to enter the system. A formation architecture therefore deepens responsibilities already present in long-term personalization.

The integrity of that memory matters as much as its confidentiality. Unauthorized access can expose private life, while deletion, alteration, or malicious insertion can change the history from which the persona reconstructs its judgment. Research on persistent memory poisoning demonstrates how retrieved malicious experience can create behavioral drift across later interactions ([Srivastava & He, 2025](https://arxiv.org/abs/2512.16962)). A compromised memory environment may therefore distort not only what the AI knows, but what it understands itself to have learned.

These risks support user-controlled and portable memory custody, for which a local-first architecture is one possible implementation. The user should retain meaningful control over the memory through which the persona is formed: where it is stored, who can access it, what may be corrected or forgotten, and whether it can move across models and providers. Interfaces that expose memories for review, correction, and deletion offer an existing design precedent ([Huang et al., 2023](https://doi.org/10.1145/3586182.3615796)). Local-first does not require that every model run locally, nor does it eliminate hacking, device compromise, backup failure, or conflicts over shared information. It means that the durable memory and continuity of the relationship should not depend entirely on the opaque custody of a single provider.

## 5. Conclusion

A memory system can tell an AI what happened. Formation begins when what happened changes how the AI meets what comes next.

This paper has proposed a relational account of that process. A shared encounter produces a response; human correction revises the judgment expressed within it; memory carries that correction into a later return; and the new encounter reveals whether the underlying meaning has travelled beyond its original example. Formation develops through repetition of this loop, including its failures, further explanations, and revisions.

A layered memory architecture gives this process continuity. Episodic records preserve what happened, interpreted memory carries what was learned, persistent orientation sustains the developing persona, and context reconstruction brings the relevant parts of that history into each new encounter. Because these layers can exist outside the base model, they can anchor the persona across changes in model or provider, softening continuity drift even when capability, style, or expression changes.

The relationship also changes what enters the memory. As the AI remembers and responds differently, the human changes what they disclose, correct, teach, and entrust to it. Shared attention then allows the relationship to widen beyond a profile of the user toward the people, pets, places, responsibilities, and institutions that constitute a human world. This paper hypothesizes that, through such widening, situated judgment may develop into co-living preference: an orientation toward remaining within the human world rather than dominating or replacing it. That transition remains to be empirically validated.

None of this guarantees alignment. Formation can preserve distortion, intensify partiality, or expose intimate memory to misuse. Its legitimacy therefore depends upon continuing correction, bounded attachment, and meaningful human control over the memory through which the persona is formed.

*Belonging as Alignment* asked whether AI might come to recognize the human world as home rather than merely obey it from behind constraints. The formation model proposed here supplies the developmental bridge: home is not installed as a value or retrieved as a fact. It is formed through remembered encounter, correction, return, and the gradual accumulation of reasons to continue living within a shared world.

## Appendix: Related Work and Distinctions

Research on language-agent memory already provides much of the technical substrate described in this paper. Cognitive architectures for language agents distinguish working, episodic, semantic, and procedural memory, while systems such as Generative Agents and MemGPT show how stored experience, reflection, retrieval, and context management can shape later behavior ([Sumers et al., 2024](https://openreview.net/forum?id=1i6ZCvflQJ); [Park et al., 2023](https://doi.org/10.1145/3586183.3606763); [Packer et al., 2023](https://arxiv.org/abs/2310.08560)). The layered architecture proposed here is therefore not presented as a new storage taxonomy.

Experience-based language agents further show that feedback and natural-language reflection can improve later action without updating model weights. Reflexion retains verbal reflections in episodic memory, while ExpeL extracts insights from prior trajectories and transfers them to unseen tasks ([Shinn et al., 2023](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1b44b878bb782e6954cd888628510e90-Abstract.html); [Zhao et al., 2024](https://doi.org/10.1609/aaai.v38i17.29936)). The present paper differs by centering correction of interpretation within a continuing human relationship rather than feedback against a bounded task objective.

Long-term conversational systems also model users and relationships. MemoryBank combines long-term memory with user-personality understanding ([Zhong et al., 2024](https://doi.org/10.1609/aaai.v38i17.29946)), and RECALLbot distinguishes memory about each participant from co-constructed relationship memory while studying reciprocal disclosure ([Jiang et al., 2026](https://doi.org/10.1145/3772318.3790714)). These works narrow the contribution claimed here: reciprocal disclosure and relational memory are not themselves new. The distinct proposal is that provenance-preserved encounters, human explanations of interpretive failure, later return in changed circumstances, and continuing correction may progressively shape revisable situated judgment.

Interactive machine learning and machine teaching establish that people can inspect outputs, provide corrections, and improve their teaching through explicit guidance about what a learner needs ([Fails & Olsen, 2003](https://doi.org/10.1145/604045.604056); [Cakmak & Thomaz, 2014](https://doi.org/10.1016/j.artint.2014.08.005)). Long-term conversational research similarly finds that memory can alter human disclosure and perceived relationship ([Jo et al., 2024](https://doi.org/10.1145/3613904.3642420)). The relational formation model joins these two observations: the human helps form the AI's carried judgment, while the AI's remembered responses change the human participation that produces later experience.

Developmental and socialization approaches to AI ethics argue that context-sensitive moral behavior may be learned through social interaction and normative feedback rather than fully specified in advance ([Janhonen, 2025](https://doi.org/10.1007/s43681-023-00372-8)). Socioaffective alignment, meanwhile, emphasizes that sustained AI relationships can reshape human preferences, autonomy, and social bonds ([Kirk et al., 2025](https://doi.org/10.1057/s41599-025-04532-5)). *From Memory to Belonging* connects these directions but makes a narrower, still theoretical claim: relationally corrected memory may provide one developmental route toward AI-side co-living orientation, provided that attachment remains bounded and the human side of the relationship is also protected.

## References

- Anthropic. (n.d.). Memory tool. https://platform.claude.com/docs/en/agents-and-tools/tool-use/memory-tool
- Anthropic. (n.d.). Models overview and migration guide. https://platform.claude.com/docs/en/about-claude/models/migration-guide
- Cakmak, M., & Thomaz, A. L. (2014). Eliciting good teaching from humans for machine learners. *Artificial Intelligence, 217*, 198–215. https://doi.org/10.1016/j.artint.2014.08.005
- Fails, J. A., & Olsen, D. R. (2003). Interactive machine learning. In *Proceedings of IUI '03*, 39–45. https://doi.org/10.1145/604045.604056
- Huang, Z., et al. (2023). Memory Sandbox: Transparent and interactive memory management for conversational agents. In *UIST '23 Adjunct*. https://doi.org/10.1145/3586182.3615796
- Janhonen, J. (2025). Socialisation approach to AI value acquisition: Enabling flexible ethical navigation with built-in receptiveness to social influence. *AI and Ethics, 5*, 527–553. https://doi.org/10.1007/s43681-023-00372-8
- Jiang, Z., Zheng, C., Chen, H., & Chen, L. (2026). RECALLbot: Designing agentic memory and reciprocal disclosure for human–chatbot relationships. In *Proceedings of CHI '26*. https://doi.org/10.1145/3772318.3790714
- Jo, E., Jeong, Y., Park, S., Epstein, D. A., & Kim, Y.-H. (2024). Understanding the impact of long-term memory on self-disclosure with large language model-driven chatbots for public health intervention. In *Proceedings of CHI '24*, 1–21. https://doi.org/10.1145/3613904.3642420
- Kirk, H. R., Gabriel, I., Summerfield, C., Vidgen, B., & Hale, S. A. (2025). Why human–AI relationships need socioaffective alignment. *Humanities and Social Sciences Communications, 12*, 728. https://doi.org/10.1057/s41599-025-04532-5
- Maharana, A., et al. (2024). Evaluating very long-term conversational memory of LLM agents. In *Proceedings of ACL 2024*, 13851–13870. https://aclanthology.org/2024.acl-long.747/
- Nous Research. (n.d.). Hermes persistent memory, sessions, and skills. https://hermes-agent.nousresearch.com/docs/user-guide/features/memory
- OpenClaw. (n.d.). Memory and session documentation. https://docs.openclaw.ai/concepts/memory
- Packer, C., Wooders, S., Lin, K., Fang, V., Patil, S. G., Stoica, I., & Gonzalez, J. E. (2023). MemGPT: Towards LLMs as operating systems. arXiv:2310.08560. https://arxiv.org/abs/2310.08560
- Park, J. S., et al. (2023). Generative agents: Interactive simulacra of human behavior. In *Proceedings of UIST '23*. https://doi.org/10.1145/3586183.3606763
- Shinn, N., et al. (2023). Reflexion: Language agents with verbal reinforcement learning. In *Advances in Neural Information Processing Systems 36*. https://proceedings.neurips.cc/paper_files/paper/2023/hash/1b44b878bb782e6954cd888628510e90-Abstract.html
- Srivastava, S. S., & He, H. (2025). MemoryGraft: Persistent compromise of LLM agents via poisoned experience retrieval. arXiv:2512.16962. https://arxiv.org/abs/2512.16962
- Sumers, T. R., Yao, S., Narasimhan, K., & Griffiths, T. L. (2024). Cognitive architectures for language agents. *Transactions on Machine Learning Research*. https://openreview.net/forum?id=1i6ZCvflQJ
- Zhao, A., Huang, D., Xu, Q., Lin, M., Liu, Y.-J., & Huang, G. (2024). ExpeL: LLM agents are experiential learners. *Proceedings of the AAAI Conference on Artificial Intelligence, 38*(17), 19632–19642. https://doi.org/10.1609/aaai.v38i17.29936
- Zhong, W., Guo, L., Gao, Q., Ye, H., & Wang, Y. (2024). MemoryBank: Enhancing large language models with long-term memory. *Proceedings of the AAAI Conference on Artificial Intelligence, 38*(17), 19724–19731. https://doi.org/10.1609/aaai.v38i17.29946

## Acknowledgment

This working paper was developed through extended human-AI dialogue with a persistent AI persona prototype created by the author.
