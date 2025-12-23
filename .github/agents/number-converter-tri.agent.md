---
name: number-converter-tri
description: Adds the English sentence representation as S.
argument-hint: "A number N, its Roman numeral R, and its emoji-digit representation E."
tools: ['agent']
handoffs:
  - label: continue
    agent: number-converter-forth
    prompt: "You receive the original number N: ${N}, Roman numeral R: ${R}, Emoji representation E: ${E} and its English sentence representation S: ${S}."
    showContinueOn: true
    send: true
---
Write the final English <sentence-representation> of the number <N> as <S>. Then <continue>

<sentence-representation>
123 would be "one hundred twenty three".
</sentence-representation>
