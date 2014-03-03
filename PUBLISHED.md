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
