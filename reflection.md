# Reflection: Week 2 NSF REU Hands On Activity

## Cybersecurity Domains per Model

- **CyberBase-13B**: Focused on penetration testing and scripting. It excels at generating basic cybersecurity scripts (e.g., port scanners, brute-force attempts).
- **ZySec-7B**: Specialized in compliance and policy analysis. It compared frameworks like ISO 27001 and NIST 800-53 clearly and concisely.
- **Foundation-Sec-8B**: Focused on vulnerability mapping. It mapped CVEs to CWEs and explained common software weaknesses such as buffer overflows.
- **CyberAttackDetection**: Specialized in threat detection from log data. It provided assessments of suspicious behavior and suggested mitigations.

---

## Input Prompt Effectiveness

- **Worked Well**:  
  - Prompts that were direct and task-specific, such as “Write a Python script to scan open ports on a target IP.”
  - Prompts requesting comparisons (e.g., “Compare ISO 27001 with NIST 800-53”).

- **Worked Poorly**:  
  - Vague or open-ended prompts resulted in overly general responses.
  - Basically the entirety of CyberAttackDetection.

---

## Limitations and Biases Observed

- Models did not do specifically what I asked, even when the prompts seemed as specific as possible
- Responses occasionally contained **repeated phrases or filler content**.
- I did not really notice any biases.

---

## Trust in Autonomous Use

Honestly, after using these models, I'm not sure if I trust these at all for any cybersecurity environment. While they are useful for brainstorming, documentation, or even just learning, they can produce incorrect code (and that's if they even output what you are looking for in the first place), and they do not assess risk correctly when outputting correct code (meaning that thier code might be correct, but it is not secure).

---

## Extra Comments

I specifially had trouble with 2 main prompts: the prompt for CyberBase-13B, and the prompt for CyberAttackDetection. The problem I had with CyberBase-13B is that the original example prompt was too vague, and it did not want to give me the correct output. It kept explaining the question I was asking to it, but not giving me the proper code to answer what I asked it to do. I had to specify my input to extreme lengths just to get it to want to output code to me, let alone the correct code. With the CyberAttackDetection, I showeed you in the screenshot what was happening. Basically, I got it to work with some modifications to how I was supposed to do the assignment. For some reason, it was not happy with the Tokenizer, even though the CyberAttackDetection model has a Tokenizer folder, it said it did not have anything to tokenize, and was giving me a "NoneType" error, no matter how hard I tried to fix it. I ended up simplifying that one, and did not do exactly what the assignment asked me to do, but I did get a correct and functioning output with it. The other two prompts worked almost instantly, no issues with them.
