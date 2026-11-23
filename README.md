# Theory of Computer Science: Self-Learning with JFLAP

This folder contains 30 JFLAP examples for self-learning the theory of computation: automata, regular and context-free grammars, parsing, Turing machines, and L-systems. Each `.jff` file is a ready-to-open JFLAP project that you can run, convert, and test.

## About JFLAP

JFLAP is software for experimenting with formal languages. It covers nondeterministic finite automata, nondeterministic pushdown automata, multi-tape Turing machines, several types of grammars, parsing, and L-systems. You can build and test examples, and you can also watch construction proofs convert one form into another, such as an NFA to a DFA, then to a minimal DFA, then to a regular expression or regular grammar.

- Download JFLAP: https://www.jflap.org/modules/
- What JFLAP can do: https://www.jflap.org/whatis.html

JFLAP needs Java installed on your computer.

## Setup

1. Install Java if you do not already have it.
2. Download and run JFLAP from https://www.jflap.org/modules/.
3. In JFLAP, open a file with **File → Open** and choose a `.jff` file from this folder.

## Files

| # | Topic | File | What the example shows |
|---|-------|------|------------------------|
| 1 | Deterministic Finite Automata | `24_PoorvajaJoshi_deterministic_finite_automata_01-11-26.jff` | DFA accepting strings over {a,b} that end in "ab" |
| 2 | Nondeterministic Finite Automata | `24_PoorvajaJoshi_nondeterministic_finite_automata_01-11-26.jff` | NFA accepting strings that end in "ab" |
| 3 | NFA to DFA Conversion | `24_PoorvajaJoshi_nfa_to_dfa_conversion_01-11-26.jff` | NFA for strings whose second-to-last symbol is "a" |
| 4 | DFA Minimization | `24_PoorvajaJoshi_dfa_minimization_01-11-26.jff` | DFA with two equivalent states that minimize to 2 states |
| 5 | DFA to Regular Grammar Conversion | `24_PoorvajaJoshi_dfa_to_regular_grammar_01-11-26.jff` | DFA for strings with an even number of a's |
| 6 | DFA to Regular Expression Conversion | `24_PoorvajaJoshi_dfa_to_regular_expression_01-11-26.jff` | DFA for strings starting with "a" |
| 7 | Combining Automata | `24_PoorvajaJoshi_combining_automata_01-11-26.jff` | DFA for strings containing "aa", for union or concatenation with another automaton |
| 8 | Regular Expression | `24_PoorvajaJoshi_regular_expression_01-11-26.jff` | Regular expression `(a|b)*abb` |
| 9 | Regular Expression to DFA Conversion | `24_PoorvajaJoshi_regex_to_dfa_01-11-26.jff` | Regular expression `(ab|b)*a` |
| 10 | Regular Expression Identities | `24_PoorvajaJoshi_regular_expression_identities_01-11-26.jff` | Regular expression `(a|b)*` for checking identities |
| 11 | Regular Grammar | `24_PoorvajaJoshi_regular_grammar_01-11-26.jff` | Right-linear grammar for a*ba |
| 12 | Regular Grammar to DFA Conversion | `24_PoorvajaJoshi_regular_grammar_to_dfa_01-11-26.jff` | Regular grammar to convert into a DFA |
| 13 | DFA Relationship to Grep | `24_PoorvajaJoshi_dfa_grep_abb_01-11-26.jff` | DFA for `(a|b)*abb`, the pattern that grep matches |
| 14 | Mealy Machine | `24_PoorvajaJoshi_mealy_detect_01_01-11-26.jff` | Mealy machine that outputs 1 when "01" is completed |
| 15 | Moore Machine | `24_PoorvajaJoshi_moore_detect_01_01-11-26.jff` | Moore machine that outputs 1 right after "01" is seen |
| 16 | Context-free Grammar | `24_PoorvajaJoshi_context_free_grammar_01-11-26.jff` | S → aSb \| λ, which generates aⁿbⁿ |
| 17 | Pushdown Automata | `24_PoorvajaJoshi_pushdown_automaton_01-11-26.jff` | PDA accepting aⁿbⁿ (n ≥ 1) by final state |
| 18 | NPDA to CFG Conversion | `24_PoorvajaJoshi_npda_even_palindrome_01-11-26.jff` | NPDA for even palindromes, to convert into a CFG |
| 19 | CFG to NPDA Conversion | `24_PoorvajaJoshi_cfg_balanced_parentheses_01-11-26.jff` | CFG for balanced parentheses, to convert into an NPDA |
| 20 | Context-free Grammar with Single Symbols | `24_PoorvajaJoshi_cfg_single_symbols_01-11-26.jff` | Grammar whose right-hand sides are single symbols |
| 21 | Context-free Grammar with Multiple Symbols | `24_PoorvajaJoshi_cfg_multiple_symbols_01-11-26.jff` | Grammar with multi-symbol right-hand sides, S → aAb |
| 22 | CFG in Error using User Control Parse | `24_PoorvajaJoshi_cfg_error_parse_01-11-26.jff` | Grammar S → aSb \| ab for stepping through a parse by hand |
| 23 | LL Parsing | `24_PoorvajaJoshi_ll_parsing_01-11-26.jff` | LL(1) grammar for arithmetic expressions |
| 24 | LR Parsing | `24_PoorvajaJoshi_lr_parsing_01-11-26.jff` | LR grammar E → E+T \| T, T → a |
| 25 | CYK Parsing | `24_PoorvajaJoshi_cyk_parsing_01-11-26.jff` | Grammar in Chomsky Normal Form for CYK parsing |
| 26 | One-Tape Turing Machine | `24_PoorvajaJoshi_one_tape_turing_machine_01-11-26.jff` | One-tape TM that replaces every a with b |
| 27 | Multi-Tape Turing Machine | `24_PoorvajaJoshi_multi_tape_turing_machine_01-11-26.jff` | Two-tape TM that copies input to the second tape |
| 28 | Turing Machine Building Blocks | `24_PoorvajaJoshi_turing_building_block_01-11-26.jff` | TM that moves right to the first blank, a reusable subroutine |
| 29 | Unrestricted Grammar | `24_PoorvajaJoshi_unrestricted_grammar_01-11-26.jff` | Unrestricted grammar that generates aⁿbⁿcⁿ |
| 30 | L-System Simple | `24_PoorvajaJoshi_lsystem_simple_01-11-26.jff` | L-system with axiom A and rules A → AB, B → A |

## Suggested Learning Path

1. **Finite automata (1–7):** Open each DFA and NFA, step through strings, then run NFA to DFA conversion and DFA minimization. Use the conversion options to see DFA to regular grammar and DFA to regular expression.
2. **Regular expressions (8–10):** Test strings against each expression, convert the expression to a DFA, and check identities by comparing the automata.
3. **Regular grammars and grep (11–13):** Convert grammars to DFAs and compare the DFA for `(a|b)*abb` with grep's behavior on sample text.
4. **Transducers (14–15):** Run the Mealy and Moore machines on input strings and compare their outputs.
5. **Context-free languages (16–22):** Test grammars, convert between PDAs and CFGs, and step through parses using user-controlled parsing.
6. **Parsing (23–25):** Run LL, LR, and CYK parsers on the given grammars and compare their results.
7. **Turing machines (26–28):** Trace the one-tape and multi-tape machines step by step, and reuse the building block in other machines.
8. **Grammars and L-systems (29–30):** Derive strings from the unrestricted grammar and generate successive L-system strings.

## Notes

- Files 1–25 and 29 are in JFLAP's standard formats.
- Files 26–28 (Turing machines) and 30 (L-system) were written by hand and may need small fixes in JFLAP. Open them in JFLAP and compare them with a machine you build in the editor.
- File 27 (multi-tape TM) may need to be redrawn in JFLAP's multi-tape editor.
- File 14 (Mealy) and 15 (Moore) use output tags written by hand. If JFLAP rejects them, rebuild the machine in its editor.
- Files 08–10 use the regular expression format. If JFLAP does not load them, enter the expression in JFLAP's regular expression editor and save it.
- Topics 31–35 (L-System Complicated, Regular Pumping Lemma, Context-free Pumping Lemma, CFG to Chomsky Normal Form, and Thoughts on Visualization) are not included yet.
- Unsolved exercises from the reference books in the syllabus can be added as extra files.

## Source

Topic list and JFLAP materials follow the course syllabus and https://www.jflap.org/modules/.
