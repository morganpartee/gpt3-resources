I experimented a ton with JSON before giving up and using something more esoteric (Which honestly, is all a red flag. That's reinventing the wheel - And when you do that, it's probably not super round.)

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I mostly write GPT-3 prompts in a formal subset of JavaScript consisting only of top-level assignments of JSON literals to variables, using a stop sequence of &quot;;⏎&quot; (semicolon, newline) so generations can be parsed as JSON.<br><br>Also, here&#39;s the wiki on Taken 4: The Musical: <a href="https://t.co/AXS6z8ktUR">pic.twitter.com/AXS6z8ktUR</a></p>&mdash; Riley Goodside (@goodside) <a href="https://twitter.com/goodside/status/1608329313425686530?ref_src=twsrc%5Etfw">December 29, 2022</a></blockquote> 

I think the difference here is Riley gets it compliant by showing it how - the whole prompt is strict JSON. Worth remembering, it mimics really well.

---

Oh my god, okay so maybe this whole repo is just going to become a Riley fan letter, this is what inspired it, (and is the format I used in codegpt for multi-file stuff)

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Here’s a more esoteric method to get quote safety without escaping. Here we use an ad hoc, indentation-based method of quoting strings so we can use simple colon labels without fear of newlines in inputs: <a href="https://t.co/G1EnCZIFm5">pic.twitter.com/G1EnCZIFm5</a></p>&mdash; Riley Goodside (@goodside) <a href="https://twitter.com/goodside/status/1557227829145882624?ref_src=twsrc%5Etfw">August 10, 2022</a></blockquote> 

[CodeGPT Ref](https://github.com/morganpartee/codegpt/blob/main/codegpt/gpt_interface.py#L50)

Honestly requiring this output format wasn't the biggest improvement in accuracy - Putting the code and prompt behind '> 's is what really did it - The two together is enough reinforcement that it's pretty damn reliable.