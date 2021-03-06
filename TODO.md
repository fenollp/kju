# To do

## Grammar
* Devise grammar for `-callback`s
    * `callback`
* Note: unused common ASCII operators: `%`, `^`, `&`, `~`, `backquote`, `;`, `\`
* `|>`-notation for funs & comprehensions
    * Would it need `∘` | `º` ?
* Restrict “holes” to inside pipes? They have to wrap around the uppermost `expr`…
* Turn `try…of…catch…end` into `case…of…catch…end` to hinder `case catch`-ing code?
* `-include`, `-include_lib` as `#include`*
* Lex atoms: `^[0-9][^\s]+`
* Add grammar for preprocessor, if possible. (`#` on col0, scrambled text between parens, …)
* Move `and` & `or` precedences' has high as their exception-gulping counterparts (more power)
    * because `C == $\n or C == $\t` > `(C == $\n) or (C == $\t)`
* Parse `(Mod:)?F/N` matching on modules' functions (as special a maching rule as exceptions)

## Parser
* Haskell: [uu-parsinglib](http://hackage.haskell.org/package/uu-parsinglib) or `parsec` + lexer + pretty_printer
* Or just look for a C backend to ANTLR4. Or an Erlang one. Or an haskell one.

## Documentation
* Put up a pretty and quick one-pager™ on [fenollp.github.io/er](http://fenollp.github.io/er)
* Clean up `README.md` and clarify direction.
* Write a syntax colouring plugin for Pygments or emacs
