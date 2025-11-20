EBNF (Extended Backus-Naur Form) is a notation for describing the syntax of languages (programming languages included). Since Pisan is simple and consistent enough, it's possible to describe it's whole structural syntax using it:


```EBNF
text = sentence, { sentence };

sentence = [subject], verb, [modifier], [object];

subject = pronoun | noun, [adjective];
    
    pronoun = "mi" | "mis" | "tu" | "tus" | "le", "les";
    
    adjective = "TODO";

verb = [negation], mood, noun, [tense], [aspect];
    
    negation = "no" | "si";
    
    mood = "ni" | "ka" | "go";
    
    tense = "pa" | "fu";
    
    aspect = "na";

modifier = "TODO";

object = "li", noun;
```