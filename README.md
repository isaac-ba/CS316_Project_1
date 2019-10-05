CS 316 : Principles of Progrmaming Languages 

Project 1: Lexical Analyzer 

EBNF: 

⟨digit⟩ → 0 | 1 | ... | 9

⟨unsigned int⟩ → {⟨digit⟩}+

⟨signed int⟩ → (+|−) {⟨digit⟩}+

⟨float⟩ → [+|−] ( {⟨digit⟩}+ "." {⟨digit⟩} | "." {⟨digit⟩}+ )

⟨floatE⟩ → ⟨float⟩ (e|E) [+|−] {⟨digit⟩}+

⟨instruction name⟩ → "iconst" | "iload" | "istore" | "fconst" | "fload" | "fstore" |
                                    "iadd" | "isub" | "imul" | "idiv" | "fadd" | "fsub" | "fmul" | "fdiv" |
                                    "intToFloat" |
                                    "icmpeq" | "icmpne" | "icmplt" | "icmple" | "icmpgt" | "icmpge" |
                                    "fcmpeq" | "fcmpne" | "fcmplt" | "fcmple" | "fcmpgt" | "fcmpge" |
                                    "goto" | "invoke" | "return" | "ireturn" | "freturn" | "print"
⟨colon⟩ → ":"

⟨comma⟩ → ","


DFA:
<p>
  <img src="/Users/yitz/Desktop/Screen Shot 2019-10-04 at 8.47.25 AM.png" width="500" alt="accessibility text">
</p>

# Java
