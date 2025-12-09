# EBNF
---
EBNF (Extended Backus-Naur Form) is a notation for describing the syntax of languages (programming languages included). Since Pisan is simple and consistent enough, it's possible to describe it's whole structural syntax using it:


```EBNF
text = sentence, { sentence };

sentence = [linker], [subject], verb, [modifier], [indirect_object], [direct_object];

subject = pronoun | noun, [adjective];
    
    pronoun = "mi" | "mis" | "tu" | "tus" | "le", "les";
    
    adjective = "TODO";

verb = [negation], mood, noun, [tense], [aspect];
    
    negation = "no" | "si";
    
    mood = "ni" | "ka" | "go";
    
    tense = "pa" | "fu";
    
    aspect = "na" | "te" | "ge";

modifier = "TODO";

indirect_object = "ke", noun;

direct_object = "li", noun;
```