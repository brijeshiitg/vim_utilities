# Minimal instructions to get started with customized vim:

- Copy **.vimrc** file to location **~/**

- Copy **'colors/monokai.vim'** to location **'~/.vim/colors/**

- Open **.vimrc** file and add **colorscheme monokai**

- In order to use the plugins, run *PluginInstall* as follows:
	
	- open *vim*
	
	- Type **:PluginInstall** 

	- Done!


# Few basic shortcuts for vim:

## Navigation:
#### Following are a few basic navigation commands:
	>
	> - **j** : down
	> - **k** : up
	> - **h** : left
	> - **l** : right
	> - **w** : a word forward
	> - **b** : a word backward
	> - **<shift> + i** : beginning of line + INSERT mode
	> - **<shift> + a** : end of the line + INSERT mode
	> - **f<char>** : jumps forward to top of the *char* 
	> - **F<char>** : jumps backward to top of the *char* 
	> - **t<char>** : jumps forward to the *char* 
	> - **T<char>** : jumps backward to the *char* 
	> - **<ctrl>+u** : page up 
	> - **<ctrl>+d** : page down
	> - **<ctrl>+y** : one line up
	> - **<ctrl>+e** : one line down


## Copy / Cut / Paste / Delete:

	 **yy** : yank or copy the current line
	 **dw** : cut or delete the current word
	 **dd** : cut or delete the current line
	 **p** : paste below to the current line
	 **P** : paste above to the current line
	 **x** : delete a single character
	 **s** : delete a single character + INSERT mode
	 **<shift> + d** : delete the rest of the lin
	 **<shift> + c** : delete the rest of the line + INSERT mode
	 **<shift> + s** : delete the intire line + INSERT mode
	 **dt<char>** : delete upto *char*
	 **ct<char>** : delete upto *char* + INSERT mode


## Copy / cut / delete a block of code:

	step1: **<shift>+v** : highlight the line
	step2: start pressing **j** to select downward (alternatively, **k** to select updward)
	step3: **y** to yank (alternatively, **d** to delete) the selected block
	
	Note: use *v* instead of *<shift+v>* to start highlighting from the current word


## Undo / Redo:

	 **u** : undo last command
	 **<ctrl>+r** : redo last command


## Search a text:
	 **/<word>** : will highlight the occurences of *word* in the text
		 press **n** to goto the next occurence
		 press **<shift>+n** to goto the previous occurence
	 ** * ** : searches forward the occurence of the current word	
	 ** # ** : searches backward the occurence of the current word	


## Find and replace:

	 **%s/<search_text>/<replace_text>/g** : replaces *all* the occurences of *<search_text>* with *<replace_text>*
	 **%s/<search_text>/<replace_text>/gi** : replaces *all* the occurences of *<search_text>* with *<replace_text>* (Case-insensitive)
	 **%s/<search_text>/<replace_text>/gc** : asks before replacing *each* occurence of *<search_text>* with *<replace_text>*
	 **%s/<search_text>/<replace_text>/gci** : asks before replacing *each* occurence of *<search_text>* with *<replace_text>* (Case-insensitive)


## Insert a line above or below the current line:

	 **o** : new line with indentation below current line
	 **<shift>+o** : new line with indentation above current line


## Commenting block of python code:
	step1: **<ctrl>+v**
	step2: keep pressing **j** to select downward (alternatively, press **k** to select upward)
	step3: **<shift>+i**
	step4: press **#** for python comment (alternatively, delete # for removeing comment)
	step5: press **<ESC>**	


## Bonus:

In INSERT model keep pressing **<ctrl> + y** to replicate previous line word by word
