C== (Sea, Eck, Eck)

<marquee>[REDUCE EDP] -- [A MODERN C FOR THE MODERN WORLD]</marquee>

C== is born out of frustration with existing languages and environments for systems programming. Programming has become too difficult and the choice of language is partly to blame. One has to choose elegance or practality. Programmers who choose practicality over elegance are using C. However, C has some serious legacy warts that cause Endless Programmer Despair (EDP). To correct these issues, C== provides a new language in the C family with a modern core while still keeping the same C elegance and power. C== is mostly in the C family (basic syntax), with significant input from the Ruby/Basic family (friendly delimiters), plus some ideas from C++. In every respect the language was designed by thinking about what programmers do and how to make programming, at least the kind of programming we do, free of EDP, which means more fun! C== is an attempt to combine the ease of programming of an interpreted, dynamically typed language with the efficiency and safety of a statically typed, compiled language. It also aims to support the modern constructs that programmers have come to love. Finally, it is intended to be fast: it should take at most a few seconds to compile. To meet these goals required addressing a number of linguistic issues: an expressive but lightweight type system; succint syntactic abstractions; a rigid standard; and so on. C== attempts to reduce the amount of typing in both senses of the word. Throughout its design, we have tried to reduce clutter and complexity. Programmers are most familiar with procedural languages, particularly from the C family. The need to be productive quickly in a new language means that the language cannot be too radical. This applies here the same as it does with all programmer tools. By keeping the set of new things small, C== is an easy addition to any programmer's toolbox. We hope you'll enjoy using it as much as we enjoyed making it. There's a hacker in all of us and a community inside of all happy us hacker now hacking! :)

Intro:

Write single line blocks with brace delimiters.

````
	int main { printf("Hello, World\n"); }



Write multi line blocks with bareword delimiters.

````
	int main BEGIN
	    printf("Hello, World\n");
	    return 0;
	END



Don't mix brackets and barewords for the same block! This "feature" will be removed in future versions!

````
	// DANGER! THIS WILL BE REMOVED IN FUTURE VERSIONS OF THE LANGUAGE!
	int main BEGIN return 0; }
	int main { return 0; END
