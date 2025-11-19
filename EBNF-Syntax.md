EBNF (Extended Backus-Naur Form) is a notation for describing the syntax of languages (programming languages included). Since Pisan is simple and consistent enough, it's possible to describe it's whole structural syntax using it:


```EBNF
text = sentence, { sentence };




sentence = [subject], verbal_structure, [verb_complement], [question_specifier];




verb_structure = verb_mood, noun, [verb_tense];

verb_mood = "ni" | "ka" | "go";
verb_tense = "pa" | "na" | "fu";


verb_complement = "ta", noun;




subject = pronoun | ...;
pronoun = ("mi" | "mis") | ("tu" | "tus") | ("le", "les");
noun = ...;




question_specifier = "ka";


```