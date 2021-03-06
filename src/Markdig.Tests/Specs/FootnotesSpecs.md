# Extensions

This section describes the different extensions supported:

## Footontes

Allows footnotes using the following syntax (taken from pandoc example):

```````````````````````````````` example
Here is a footnote reference,[^1] and another.[^longnote]

This is another reference to [^1]

[^1]: Here is the footnote.

And another reference to [^longnote]

[^longnote]: Here's one with multiple blocks.

    Subsequent paragraphs are indented to show that they
belong to the previous footnote.

    > This is a block quote
    > Inside a footnote

        { some.code }

    The whole paragraph can be indented, or just the first
    line.  In this way, multi-paragraph footnotes work like
    multi-paragraph list items.

This paragraph won't be part of the note, because it
isn't indented.
.
<p>Here is a footnote reference,<a id="fnref:1" href="#fn:1" class="footnote-ref"><sup>1</sup></a> and another.<a id="fnref:3" href="#fn:2" class="footnote-ref"><sup>2</sup></a></p>
<p>This is another reference to <a id="fnref:2" href="#fn:1" class="footnote-ref"><sup>1</sup></a></p>
<p>And another reference to <a id="fnref:4" href="#fn:2" class="footnote-ref"><sup>2</sup></a></p>
<p>This paragraph won't be part of the note, because it
isn't indented.</p>
<div class="footnotes">
<hr />
<ol>
<li id="fn:1">
<p>Here is the footnote.<a href="#fnref:1" class="footnote-back-ref">&#8617;</a><a href="#fnref:2" class="footnote-back-ref">&#8617;</a></p>
</li>
<li id="fn:2">
<p>Here's one with multiple blocks.</p>
<p>Subsequent paragraphs are indented to show that they
belong to the previous footnote.</p>
<blockquote>
<p>This is a block quote
Inside a footnote</p>
</blockquote>
<pre><code>{ some.code }
</code></pre>
<p>The whole paragraph can be indented, or just the first
line.  In this way, multi-paragraph footnotes work like
multi-paragraph list items.<a href="#fnref:3" class="footnote-back-ref">&#8617;</a><a href="#fnref:4" class="footnote-back-ref">&#8617;</a></p>
</li>
</ol>
</div>
````````````````````````````````

