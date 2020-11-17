---
topic: how-all-this-works
time: 11-17 1348
place: jujuroom 43
rambles: its nice to finally get to this
category: blogpost
---

so how does any of this work?  
great question

right now i am typing in neovim in a tmux session in my terminal

i am going to build my blog from scratch right now

dont worry i have alot of shortcuts

		is this a comment? if so,
		h1 is site technomad, h2 is page blog, h3 is article title,
		h4 is h1 h5 is h2
		because this header isnt important im gonna give it h5

##### where to start

the first thing i need to do is clone my tms  
this time i wanted to try to include it as a submodule?  
i think that will help with splitting the content  
but then im going to need to reconfig the whole stack  
sweeeeet

##### some first moves

mkdir tm-blog  
add this file in there

		probably gonna add the whole rd, search for some yaml
		just cp'd it for now, upgrade to ln -s?

		do i just submodule tms in now?
			that might work

went up on github, created a new repo: wommy/technomad-blog

copied it again to readme,  
gonna push

##### tidied, gonna repush

ok it looks nice now,

next up is to require in tms somehow  
im aiming to use a submodule
template directory is nice, but it really complicates the folder structure

this link worked out real good 
<https://git-scm.com/book/en/v2/Git-Tools-Submodules#_starting_submodules>

		git submodule add git@github.com:wommy/technomad-stack.git

this is working lovingly,  
gonna push quick

##### whats next

i think i need to set up 11ty to work with content

right now im just gonna copy it  

		big upgrade >> link that

wait do i just make a new package.json that copies it in and runs the submodule  
no, thats step 2  

		cp content technomad-stack/11ty/


