**# Monday.com-Python-API**
In this repo I'll post projects for read, process and write data from / to Monday.com boards

*PROJECT 1: Making a Clean Pandas DataFrame from a Monday.com Board*

This project started as a simples study in my work hours just to train my Python skills and learn the basics of API's.
After at least 5h of coding, through several days, and help from my dear professor Andre from ADA
(a Coding School from Brazil), I finally arrive at this version that I'm happy to share with you!

With this code you'll be able to get data from a Monday.com board, process it and turn it into a clean Pandas Data Frame.
Why "clean"? You might ask...

The Monday.com board is very clean when using it's WorkOS, but when we import data from it throug API it comes with lots
of infos that you might find useless, and every "cell" comes with the column title and text.

So one can harvest the usefull data from it, but maybe will need to clean the cells to be able to use it.

So, this code retrieves the column titles from the cells, than get ridd of'em, keeping only the values ('text').

Finally, it merges the data frame with the name column (the first column of the board), saves it into a variable and
checks it.

I hope you'll find this project usefull.

Enjoy!

ps - I'm new to API and requests, so after finishing this code, working in a version of it, I noticed that you can
select many options in the query, adding or removing params as you like, such as "id", "title" etc.

ps2 - I've come to notice that is nice to limit the number os lines you will request in the query, or you'll maybe get
an error message. Right after items, open parentesis and enter the limit as you wish, I think 500 is about the maximum
that it can get without returning a "timeout" error. ex: [...] items(limit:400) [...]
