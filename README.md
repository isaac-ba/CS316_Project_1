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
! [Image of Given DFA][https://github.com/isaac-ba/Lexical_Analyzer/blob/master/DFA.png]


# Java
