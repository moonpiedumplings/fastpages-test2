---
keywords: fastai
title: fun with dictionaries
toc: true
author: moonpie
categories: [collegeboard]
tags: [python]
nb_path: _notebooks/2022-9-01-Dictionaries.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-9-01-Dictionaries.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">f</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;players&quot;</span><span class="p">:</span><span class="s2">&quot;11 players on the field&quot;</span><span class="p">,</span>
    <span class="s2">&quot;lineman&quot;</span><span class="p">:</span> <span class="s2">&quot;The smartest players on the field&quot;</span><span class="p">,</span>
    <span class="s2">&quot;quarterback&quot;</span><span class="p">:</span> <span class="s2">&quot;The dude who throws the ball&quot;</span>
    <span class="s2">&quot;linebacker&quot;</span><span class="p">:</span> <span class="s2">&quot;They bliz a lot&quot;</span>
<span class="p">}</span>
<span class="nb">print</span><span class="p">(</span><span class="n">f</span><span class="p">[</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;query?&quot;</span><span class="p">)])</span>

<span class="c1"># This could probably be expanded more. But it doesn&#39;t include interation which the assignment requires.</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>The smartest players on the field
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">players</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">players</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;Khalid Farah&quot;</span><span class="p">,</span>
    <span class="s2">&quot;weight&quot;</span><span class="p">:</span> <span class="mi">195</span><span class="p">,</span> <span class="c1">#Weight is in pounds</span>
    <span class="s2">&quot;positions&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;linebacker&quot;</span><span class="p">]</span>
<span class="p">})</span>

<span class="n">players</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;Jeffrey Fonseca&quot;</span><span class="p">,</span>
    <span class="s2">&quot;weight&quot;</span><span class="p">:</span> <span class="mi">200</span><span class="p">,</span>
    <span class="s2">&quot;positions&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;Offensive lineman&quot;</span><span class="p">,</span> <span class="s2">&quot;Defensive Lineman&quot;</span><span class="p">]</span>
<span class="p">})</span>

<span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">players</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">p</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">],</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>

<span class="c1"># technically, this is all I need to complete the assignment. However, I may do more.</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Khalid Farah 

Jeffrey Fonseca 

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">a</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Which player&#39;s stats do you want?&quot;</span><span class="p">)</span>
<span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">players</span><span class="p">:</span>
    <span class="k">if</span> <span class="n">p</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="n">a</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;weight = &quot;</span><span class="p">,</span><span class="n">p</span><span class="p">[</span><span class="s2">&quot;weight&quot;</span><span class="p">],</span><span class="s2">&quot;pounds </span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Positions played:&quot;</span><span class="p">,</span> <span class="n">p</span><span class="p">[</span><span class="s2">&quot;positions&quot;</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>weight =  195 pounds 

Positions played: [&#39;linebacker&#39;]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">dict</span> <span class="o">=</span> <span class="p">{}</span>
<span class="nb">dict</span><span class="o">.</span><span class="n">update</span><span class="p">({</span><span class="s2">&quot;test&quot;</span><span class="p">:</span><span class="s2">&quot;value&quot;</span><span class="p">})</span>
<span class="nb">print</span><span class="p">(</span><span class="nb">dict</span><span class="p">)</span>

<span class="c1"># finally got this working. Why was this so difficult to figure out.</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>{&#39;test&#39;: &#39;value&#39;}
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">pindex</span> <span class="o">=</span> <span class="p">{}</span>

<span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">players</span><span class="p">:</span>
    <span class="n">pindex</span><span class="o">.</span><span class="n">update</span><span class="p">({</span><span class="n">p</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">]:</span> <span class="n">p</span><span class="p">})</span>

<span class="nb">print</span><span class="p">(</span><span class="n">pindex</span><span class="p">)</span>

<span class="c1"># This program creates an index for the list,to make searching faster. </span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>{&#39;Khalid Farah&#39;: {&#39;name&#39;: &#39;Khalid Farah&#39;, &#39;weight&#39;: 195, &#39;positions&#39;: [&#39;linebacker&#39;]}, &#39;Jeffrey Fonseca&#39;: {&#39;name&#39;: &#39;Jeffrey Fonseca&#39;, &#39;weight&#39;: 200, &#39;positions&#39;: [&#39;Offensive lineman&#39;, &#39;Defensive Lineman&#39;]}}
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Right now there is no speed difference, but when working with bigger stores of info, for loops through are tedious</span>

<span class="n">a</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;player name?&quot;</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;weight=&quot;</span><span class="p">,</span><span class="n">pindex</span><span class="p">[</span><span class="n">a</span><span class="p">][</span><span class="s2">&quot;weight&quot;</span><span class="p">],</span><span class="s2">&quot;pounds</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;positions=&quot;</span><span class="p">,</span><span class="n">pindex</span><span class="p">[</span><span class="n">a</span><span class="p">][</span><span class="s2">&quot;positions&quot;</span><span class="p">])</span>

<span class="c1"># maybe creating dictionary of dictionaries would have been easier...</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>weight= 200 pounds

positions= [&#39;Offensive lineman&#39;, &#39;Defensive Lineman&#39;]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

