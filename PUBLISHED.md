List of all published tips. See [vim weekly](http://www.vimweekly.com/) for archives.

| **Tip** | **Code** | **Description** | **Summary** | **Source** | 
| :------------- | :------- | :-------------- | :---------- | :--------- |
| 1 | `:undol :undolist`| To view the list of the changes that happened to your doucument try this vim command |List the leafs in the tree of changes | vim manual|
|2|`:undo {N}`|Revert back to change number {N} where N is a number in your undo list|Revert to change in time|vim manual|
|3|`:earlier {N}f`|Go to older text state {N} file writes before. When changes were made since the last write :earlier 1f will revert the text to the state when it was written. Otherwise it will go to the write before that. When at the state of the first file write, or when the file was not written, :earlier 1f will go to before the first change.|Going back to an earlier file state|vim manual|
|4|`g+ g-`|Moving foward and backward in your change list|Navigating the change list|vim manual|
|5|`:later {N}f`|Go to newer text state {N} file writes later. When at the state of the last file write, :later 1f will go to the newest text state.|Going to an earlier file state|vim manual|
|6|`:set spell`|Enable spell checking to allow vim to check for typos, note that this only available in vim compiled with syntax support|Set spell checking in vim|[tawheed](http://www.tawheedraheem.com/)|
|7|`z=`|Once you VIM has discoreved your typos, you can put your cursor under the mispelled word and press the keys below to see for possible correction matches|Auto correct suggestion|[tawheed](http://www.tawheedraheem.com/)|
|8|`/^\n\{3}`|Find 3 empty lines in the current file, replace the number 3 with the desired number of empty lines that you would like|Finding empty lines in file|[zzapper](http://rayninfo.co.uk/vimtips.html)|
|9|`` `a``|go to position of bookmark a|Going to you saved bookmark|[csnipp](http://csnipp.com/s/69)|
|10|`ma`|make a bookmark named "a" at the current cursor position, note that you can substituite the letter "a" with other letters|Making a bookmark|[csnipp](http://csnipp.com/s/69)|
|11|`:%s/\(\s*\n\s*\)\{2,}/\r\r`|collapse multiple blank lines (regardless of quantity) into a single blank line.|collapsing blank lines|[tim](https://twitter.com/gumnos)|
|12|`:m9`| move the current line that your cursor is to line 9. You can replace the number 9 with any line number|moving lines|[tawheed](http://www.tawheedraheem.com/)|
|13|`3/joe/e+1`|find 3rd joe cursor set to End of match plus 1 [C]||[zzapper](http://rayninfo.co.uk/vimtips.html)|
|14|`Ctrl+a`|Increment the number under cursor|Increment number|[stackoverflow-vdboor](http://stackoverflow.com/questions/1218390/what-is-your-most-productive-shortcut-with-vim/2559262#2559262)|
|15|`Ctrl+x`|Decrement the number under cursor|Decrement number|[stackoverflow-vdboor](http://stackoverflow.com/questions/1218390/what-is-your-most-productive-shortcut-with-vim/2559262#2559262)|
|16|`:1,10 w outfile.txt`|Saves lines 1 to 10 to the file outfile.txt, you can change the numbers to whatever suits your needs|Saving lines to an external file|[catswhocode](http://www.catswhocode.com/blog/100-vim-commands-every-programmer-should-know)|
|17|`:1,10 w >> outfile.txt`|Appends lines 1 to 10 to outfile.txt|Appending to end of file|[catswhocode](http://www.catswhocode.com/blog/100-vim-commands-every-programmer-should-know)|
|18|`~`|Invert the case of a letter|Inverting case|[tawheed](http://www.tawheedraheem.com/)|
|19|`:X`|Encrypting a file by protecting it with a password, after you specify the encryption key you MUST write the file and save it. This is because value of your encryption key is used when text is written|Encrypt file|[tawheed](http://www.tawheedraheem.com/)|
|20|`:set key=`|To remove the encryption you can set it to empty|Remove encryption key|[tawheed](http://www.tawheedraheem.com/)|
|21 | `:ascii  :as[cii]` | print ascii value of character under the cursor| printing ascii characters | vim holy grail|
|22 | `:badd :bad[d]`| add buffer to the buffer list| adding buffer to buffer list | vim holy grail|
|23 | `:blast  :bl[ast]`| go to last buffer in the buffer list| going to the last buffer | vim holy grail|
|24 |`:tabonly` |close all tab pages except the current one |close all tab pages except the current one | vim holy grail |
|25 | `c12`|change from cursor to column 12 of current line￼|changing from current cursor |[tawheed](http://www.tawheedraheem.com/) |
|26|`:Sex`|Split window and open integrated file explorer|open file explorer |[catswhocode](http://www.catswhocode.com/blog/100-vim-commands-every-programmer-should-know)|
|27|`:r cool_file.rb`|Insert the content of cool_file.rb in buffer|Inserting contents of file|[catswhocode](http://www.catswhocode.com/blog/100-vim-commands-every-programmer-should-know)|
|28|`:23r cool_file.rb`|Insert the contents of cool_file.rb in buffer after line 23|Inserting contents of file at specific point|[catswhocode](http://www.catswhocode.com/blog/100-vim-commands-every-programmer-should-know)|
|29|`g~~`|Switch case of current line|Switching case of current line|[@gumnos](https://twitter.com/gumnos)
|30|`:sh :sh[ell]`|Start shell from vim, type exit to get back to vim |Starting a shell |[tawheed](http://www.tawheedraheem.com/)|
|31|`:reg`|Display the contents of all numbered and named registers | displaying contents of register.|[tawheed](http://www.tawheedraheem.com/)|
|32|`"jy`| Yank text into register j - you can use any of these registers {a-zA-Z0-9.%#:-"}| yanking text to named register |[tawheed](http://www.tawheedraheem.com/)|
|33|`:let @j = "puts 'some really cool string'"`| Save the text "puts 'some really cool string'" into rejister j - you can use any of these registers {a-zA-Z0-9.%#:-"}| saving text to named register |[tawheed](http://www.tawheedraheem.com/)|
|34|`:let @j .= "more cool string"`| append the text "more cool string" to rejister j | append text to register |[tawheed](http://www.tawheedraheem.com/)|
|35|`"jp`| Paste content from register j|pasting contents from register |[tawheed](http://www.tawheedraheem.com/)|
|36|`:%s#<[^>]\+>##g`|Delete HTML tags but keeps text|Delete HTML tags but keeps text|[catswhocode](http://www.catswhocode.com/blog/100-vim-commands-every-programmer-should-know)|
|37|`%s/^\(.*\)\n\1$/\1/`|Delete lines which appears twice|Delete lines which appears twice|[catswhocode](http://www.catswhocode.com/blog/100-vim-commands-every-programmer-should-know)|
|38|`vim -p fred.php joe.php`|Open the files in tabs|Opening multiple files in tabs|[zzapper](http://rayninfo.co.uk/vimtips.html)|
|39|`:s/\v<(.)(\w*)/\u\1\L\2/g`|To turn one line into title caps, make every first letter of a word uppercase|Change case of words in a sentence|[vim maual](http://vimdoc.sourceforge.net/htmldoc/change.html)|
|40|`g??`|Rot13 encode current line - Rotate each character 13 places|Rot13 encode current line|[vim maual](http://vimdoc.sourceforge.net/htmldoc/change.html)|
|41|`:1,13s/^/#/g`|Put the # in begining of lines 1 to 13, FYI - '#' is a comment in ruby so feel free to use whatever signifies a comment in your favourite language|Inserting in the begining of lines|[tawheed](http://www.tawheedraheem.com/)|
|42|`:%s/\<foo\>/bar/gc`|Change only whole words exactly matching 'foo' to 'bar'; ask for confirmation.|Replacing whole words|[vim wikia - Tip#31](http://vim.wikia.com/wiki/Search_and_replace)|
|43|`:%s/foo/\=@a/g`|Replace each occurrence of 'foo' with the contents of register 'a'.|Replace with contents of a register|[vim wikia - Tip#31](http://vim.wikia.com/wiki/Search_and_replace)|
|44|`:%s/\<foo\>//g`|On each line, delete all occurrences of the whole word "foo".|Deleting occurance in lines|[vim wikia - Tip#31](http://vim.wikia.com/wiki/Search_and_replace)|
|45|`:1,13s/^\(\w\)/\u\1/`|If the first character on lines 1 to 13 is lowercase, switch it to uppercase|Conditinally change case of line|[vim wikia - Tip#31](http://vim.wikia.com/wiki/Search_and_replace)|
|46|`vat`|Select between XML/HTML opening and closing tags|jumping between XML/HTML tags|[Ian Liu](https://plus.google.com/u/3/+IanLiuRodrigues/posts)|
|47|`SHIFT+O`|Jump between selection extremities while on visual selection|jump between extremities of XML/HTML tags|[Ian Liu](https://plus.google.com/u/3/+IanLiuRodrigues/posts)|
|48|`:%s=  *$==`|Delete end of lines that is blank|Delete end of line that is blank|[zzapper](http://rayninfo.co.uk/vimtips.html)|
|49|`:e $MYVIMRC`|Open your vimrc|open vimrc|[zzapper](http://rayninfo.co.uk/vimtips.html)|
|50|`:so $MYVIMRC`|Source your vimrc. Applying changes to current vim session without having to restart|Source vimrc|[tawheed](http://www.tawheedraheem.com/)|
|51|`%s,//\(.*\),/*\1 */,`|Change all comments that have //-this style to /* */|Change comment style|[vim wikia - Tip#1010](http://vim.wikia.com/wiki/Change_C%2B%2B_comments_to_C_comments)|
|52|`:command! -nargs=+ Evaluate :perl VIM::Msg(eval{<args>})`|Calculate and evaluate code using perl in vim|Calculate and evaluate code|[vim wikia - Tip#1359](http://vim.wikia.com/wiki/Calculator_and_code_evaluation_using_Perl)|
|52|`:command! -nargs=+ Evaluate :perl VIM::Msg(eval{<args>})`|Calculate and evaluate code using perl in vim|Calculate and evaluate code|[vim wikia - Tip#1359](http://vim.wikia.com/wiki/Calculator_and_code_evaluation_using_Perl)|
|53|`:Evaluate 1+2`|Add two numbers based on tip 52|Add two numbers|[vim wikia - Tip#1359](http://vim.wikia.com/wiki/Calculator_and_code_evaluation_using_Perl)|
|54|`:Evaluate $a=sin(0);$a==sin(0)?"equal":"not equal"`|Testing a boolean logic based on tip 52|Testing out boolean logic|[vim wikia - Tip#1359](http://vim.wikia.com/wiki/Calculator_and_code_evaluation_using_Perl)|
|55|`map <F7> <Esc>I<a href="<Esc>A"><Esc>gJA</a><Esc>`|Convert two lines (URL then TITLE) to one line - Given two lines 'http://www.example.com' and 'The Example Site' - This mapping will turn the two lines into an html link and href tag|Make an HTML anchor and href tag  Edit|[vim wikia - Tip#1178](http://vim.wikia.com/wiki/Make_an_HTML_anchor_and_href_tag)|
|56|`:silent bufdo !zip proj.zip %`|Zip All the files in your vim session|Zip files in your vim session|[vim wikia - Tip#1513](http://vim.wikia.com/wiki/Changing_all_HTML_tags_to_lowercase)||
|57|`:%s/<\([^>]*\)>/<\L\1>/g`|Changing all HTML tags to lowercase|Changing all HTML tags to lower case|[vim wikia - Tip#1513](http://vim.wikia.com/wiki/Changing_all_HTML_tags_to_lowercase)|
|58|`:9,s/\(\w*\)/(\1)/g`|If line 9 has the words `fish dog cat mouse`, this command surrounds all the words with open and closing parens|Surround words with parentheses|[vimgolf](http://www.vimgolf.com/challenges/5192f96ad8df110002000002)|
|59|`:%s/^/\=line('.').'. '`|Number each all the lines in current file. Line 1 to line n|Number List|[vimgolf](http://www.vimgolf.com/challenges/4d716c76919202611400002b)|
|60|`:s/.\{,69\};\s*\.\{,69\}\s\+/&\r/g`|break lines at 70 chars, if possible after a ; |break lines at 70 chars, if possible after a ;|[zzapper](http://rayninfo.co.uk/vimtips.html)|
|61|`nmap <silent> <leader>ch :exec 'silent !open -a "Google Chrome" % &'`|Open up current file in chrome - To invoke this mapping use leaderKey + c + h + Enter|Open current file in chrome|[shanestillwell](https://github.com/shanestillwell/dotfiles/blob/master/vimrc)|
|62|`au BufLeave,FocusLost * silent! update`|Auto save contents of a buffer when you lose focus|Autosave buffer|[Jeff](https://plus.google.com/+JeffSchwartz/posts/eNu5MV9NH5m)|
|63|`:'a,'bs/somestring//gn`|Count the number of occurances of a somestring in a file|Counting occurance of word|[zzapper](http://rayninfo.co.uk/vimtips.html)|
|64|`:g/someWord/z#.1\echo"=========="`|Display a fancy output based on your search of someWord|Display search beautifully|[brokentrain](http://gavin.brokentrain.net/projects/vimtips/vimtips.pdf)|
|65|`:g/^/m0`|Reverse the contents of a file|Reverse the contents of a    file|[brokentrain](http://gavin.brokentrain.net/projects/vimtips/vimtips.pdf)|
|66|`:lcd`|It words like !cd but only changes the cureent directory of current window|change directory of current window|vim manual|
|67|`:s#_\(\l\)#\u\1#g`|Convert snake_case to camelCase on a given line|Convert snake_case to camelCase|[Vim wikia - Tip #1602](http://vim.wikia.com/wiki/Converting_variables_to_or_from_camel_case)|
|68|`:Tohtml`|Convert entire buffer to html|Convert buffer to html|vim manaul|
|69|`let &colorcolumn=join(range(82, 255), ',')`|Enforce 82 column margin|Enforce 82 column|forgot where I found it|
|70|`:.! date`|Insert date on current line|Insert date on current line|[Stackoverflow](http://stackoverflow.com/questions/726894/what-are-the-dark-corners-of-vim-your-mom-never-told-you-about)|
|71|`map h1 yypVr=o`|When editting plain text we sometimes need to make a given line bold, vim on the other hand does not provide a way of achieving this effect. With this mapping we put "============" underneath a line to signify a heading|Marking a line as headline|Hacking Vim|
|72|`map h1 yypVr-o`|Same concept as tip#71 but this mapping is used to indicate a sub-heading by placing "-----------" underneath a given line|Marking a line as sub headline|Hacking Vim|
|73|`:jumps`|Vim keeps track of all the places that our cursor has been. If you make the cursor "jump", the position of the cursor before the jump is remembered. See `:help jump` for more information. Use the command below to show your jumps|Showing jumps in vim|vim-manual|
|74|`CTRL-O`|Going to older cursor position in jump list - Think of this like clicking on the back button on your browser|Going to older cursor position|vim-manual|
|75|`CTRL-I`|Going to new cursor position in jump list Think of this like clicking on the forward button on your browser|Going to newer cursor position|vim-manual|
