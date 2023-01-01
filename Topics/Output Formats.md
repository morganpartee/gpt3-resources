
I experimented a ton with JSON before giving up and using something more esoteric (Which honestly, is all a red flag. That's reinventing the wheel - And when you do that, it's probably not super round.)

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I mostly write GPT-3 prompts in a formal subset of JavaScript consisting only of top-level assignments of JSON literals to variables, using a stop sequence of &quot;;⏎&quot; (semicolon, newline) so generations can be parsed as JSON.<br><br>Also, here&#39;s the wiki on Taken 4: The Musical: <a href="https://t.co/AXS6z8ktUR">pic.twitter.com/AXS6z8ktUR</a></p>&mdash; Riley Goodside (@goodside) <a href="https://twitter.com/goodside/status/1608329313425686530?ref_src=twsrc%5Etfw">December 29, 2022</a></blockquote> 

I think the difference here is Riley gets it compliant by showing it how - the whole prompt is strict JSON. Worth remembering, it mimics really well.

---

Oh my god, okay so maybe this whole repo is just going to become a Riley fan letter, this is what inspired it, (and is the format I used in codegpt for multi-file stuff)

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Here’s a more esoteric method to get quote safety without escaping. Here we use an ad hoc, indentation-based method of quoting strings so we can use simple colon labels without fear of newlines in inputs: <a href="https://t.co/G1EnCZIFm5">pic.twitter.com/G1EnCZIFm5</a></p>&mdash; Riley Goodside (@goodside) <a href="https://twitter.com/goodside/status/1557227829145882624?ref_src=twsrc%5Etfw">August 10, 2022</a></blockquote> 

[CodeGPT Ref](https://github.com/morganpartee/codegpt/blob/main/codegpt/gpt_interface.py#L50)

Honestly requiring this output format wasn't the biggest improvement in accuracy - Putting the code and prompt behind '> 's is what really did it - The two together is enough reinforcement that it's pretty damn reliable.

---

[Code Generation](Code%20Generation.md), assuming prompt is a markdown file, using code blocks works great for single files:
<blockquote class="twitter-tweet"><p lang="en" dir="ltr">For code-generation tasks assuming the top-level document is Markdown and generating within code blocks with stop sequence &quot;```⏎&quot; also works well: <a href="https://t.co/755oJij4tB">pic.twitter.com/755oJij4tB</a></p>&mdash; Riley Goodside (@goodside) <a href="https://twitter.com/goodside/status/1608334443743166471?ref_src=twsrc%5Etfw">December 29, 2022</a></blockquote>

---

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Prompts defined with TypeScript/Python3 types enable specifically structured GPT output. Useful for computation chains (e.g. <a href="https://twitter.com/LangChainAI?ref_src=twsrc%5Etfw">@LangChainAI</a> ), but also generally for keeping the completion on rails.<br><br>Bonus pro-tip: GPT can&#39;t count. Use enumerated lists for specific lengths. <a href="https://t.co/OKGkZF6VyG">pic.twitter.com/OKGkZF6VyG</a></p>&mdash; Grant Slatton (@GrantSlatton) <a href="https://twitter.com/GrantSlatton/status/1609649786906619905?ref_src=twsrc%5Etfw">January 1, 2023</a></blockquote>

---

