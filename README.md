## Essential Vim motions

> This is not a Vim tutorial, but rather a compilation of what I think are the most useful Vim motions. Almost all of the keybindings are default Vim settings. The ones that are not are stated explicitly. Please read [this article](https://blog-swagatmitra.netlify.app/blog/vim) to understand the intuition behind these commands.

1. `j` - moves cursor down one line
2. `k` - moves cursor up one line
3. `h` - moves cursor to the left by one character
4. `l` - moves cursor to the right by one character
5. `u` - undo
6. `v` - enters visual mode
7. `Ctrl + r` - redo
8. `i` - enters insert mode by placing cursor to the left of current character
9. `a` - enters insert mode by placing cursor to the right of current character
10. `0` - jumps to the start of the line
11. `$` - jumps to the end of the line
12. `I` - jumps to the start of the line and enters insert mode
13. `A` - jumps to the end of the line and enters insert mode
14. `jj` - enters normal mode from insert mode (default: Esc)
15. `w` - jumps forwards (to the right) by placing the cursor on the start of each word
16. `e` - jumps forwards (to the right) by placing the cursor on the end of each word
17. `b` - jumps backwards (to the left) by placing the cursor on the start of each word
18. `ge` - jumps backwards (to the left) by placing the cursor on the end of each word
19. `x` - deletes the current character
20. `X` - deletes the character to the left of the current character
21. `(dd/cc)` - deletes current line (and enters insert mode)
22. `(d/c)0` - deletes everything from current cursor position to the start of line (and enters insert mode)
23. `D` - deletes everything from current cursor position to the end of line
24. `o` - inserts new line below current line
25. `O` - inserts new line above current line
26. `t(character)` - move to the position before the character
27. `f(character)` - move to the position of the character
28. `T(character)` - move backwards (to the left) to the right of the position of the character
29. `F(character)` - move backwards (to the left) to the position of the character
30. `Ctrl + b` - scroll up one full screen
31. `Ctrl + f` - scroll down one full screen
32. `:` - enters command mode
33. `(d/c)w` - deletes current word when cursor is on the first character (and enters insert mode)
34. `(d/c)aw` - deletes current word without leaving a space (and enters insert mode)
35. `(d/c)iw` - deletes current word and leaves a space (and enters insert mode)
36. `(d/c)ap` - deletes current paragraph (and enters insert mode)
37. `(d/c)ip` - deletes current paragraph and leaves a space (and enters insert mode)
38. `ddp` - swaps current line with the line below
39. `ddkP` - swaps current line with the line above
40. `s` - deletes current character and enters insert mode
41. `(d/c)e` - deletes all characters from current cursor position till the end of word (and enters insert mode)
42. `(d/c)b` - deletes all characters from left of the current cursor position till the beginning of word (and enters insert mode)
43. `y` - copies current character
44. `yy` - copies current line
45. `p` - paste into new line below current line
46. `P` - paste into new line above current line
47. `bi` - moves cursor to the beginning of word and enters insert mode
48. `ea` - moves cursor to the end of word and enters insert mode
49. `vae` - selects entire document
50. `(d/c)ae` - deletes entire document (and enters insert mode)
51. `yae` - copies entire document
52. `m(character)` - mark a character
53. `'(character)` - go to the marked line
54. `%` - moves to the opposite brace when cursor is on a brace
55. `yi(b/B/"/[)` - copies text inside ()/{}/""/[]
56. `(d/c)i(b/B/"/[)` - deletes text inside ()/{}/""/[] (and enters insert mode)
57. `(d/c)a(b/B/"/[)` - deletes text inside ()/{}/""/[] and the corresponding braces (and enters insert mode)
58. `~` - changes case of character
59. `ysiw(b/B/"/[)` - wraps current word in ()/{}/""/[]
60. `yss(b/B/"/[)` - wraps current line in ()/{}/""/[]
61. `{` - moves up the document to an empty line
62. `}` - moves down the document to an empty line
63. `J` - join the current line with the line below
64. `xp` - swaps current character with the character on the right
65. `cs(old)(new)` - subsitutes old braces with new
66. `ds(b/B/"/[)` - deletes the closest pair of braces which matches the brace
67. `(d/c)t(character)` - deletes everything from current cursor to the position before the cursor (and enters insert mode)
68. `(d/c)f(character)` - deletes everything from current cursor to the position of the character (and enters insert mode)
69. `>>` - indents line to the right
70. `<<` - indents line to the left
71. `r(character)` - replaces current character with character
72. `gg` - go to the top of the file
73. `G` - go to the bottom of the file
74. `vi(b/B/"/[)` - select text inside ()/{}/""/[]
75. `va(b/B/"/[)` - select text around ()/{}/""/[]
76. `W` - jump forwards (to the right) by placing the cursor on the start of each non-blank sequence of characters
77. `B` - jump backwards (to the left) by placing the cursor on the start of each non-blank sequence of characters
78. `vap` - selects entire paragraph and leaves a space
79. `vip` - selects entire paragraph without leaving a space
80. `viw` - selects the current word
81. `yiw` - copies the current word
82. `yap` - copies the current paragraph
83. `dgg` - deletes from current line to the top of file
84. `dG` - deletes from current line to the end of file
85. `gcc` - comments or uncomments current line
86. `.` - repeats the last command
87. `gd` - moves to the line/context where the current word was defined
88. `*` - search for the current word
89. `H` - move cursor to the top of screen
90. `L` - move cursor to the bottom of screen
91. `(d/c)it` - deletes text inside current html tag (and enters insert mode)
92. `(d/c)at` - deletes current html tag (and enters insert mode)
93. `(d/c)as` - deletes current sentence without leaving a space (and enters insert mode)
94. `(d/c)is` - deletes current sentence and leaves a space (and enters insert mode)
95. `n` - go to the next match of word
96. `N` - go the the previous match of word
97. `dl` - deletes current character
98. `=G` - formats the entire document
99. `(` - move backwards to the start of each sentence
100. `)` - move forwards to the start of each sentence

### Visual Mode

1. `S(brace)` - encloses selected text with braces
2. `o` - moves to the other end of the selected block
3. `ff` - leaves visual mode and enters normal mode (default: Esc)
4. `V` - enters visual block mode

### Command Mode

1. `%s/word/replace_word/(gc)` - find and replace (gc for optional prompt replacement)
2. `/word` - search forwards for word
3. `?word` - search backwards for word
4. `:w` - save
5. `:wq` - save and quit
6. `:q!` - quit without saving
