---
keywords: fastai
title: Procedures using JavaScript
comments: true
nb_path: _notebooks/2022-12-4-javascriptexamples.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-12-4-javascriptexamples.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>As we learned before, when we define procedures in python, we used "def." However, in JavaScript, we use function as opposed to def in python. Here is a basic procedure to start with. With python we would define the function with "def" but here we are using "function." After that, it is nearly the same for the rest of the program.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="kd">function</span> <span class="nx">subtraction</span><span class="p">(</span><span class="nx">a</span><span class="p">,</span><span class="nx">b</span><span class="p">)</span> <span class="p">{</span>
    <span class="k">return</span> <span class="nx">a</span> <span class="o">-</span> <span class="nx">b</span><span class="p">;</span>
  <span class="p">}</span>
  
  <span class="nx">subtraction</span><span class="p">(</span><span class="mf">10</span><span class="p">,</span><span class="mf">12</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">



<div class="output_text output_subarea output_execute_result">
<pre>-2</pre>
</div>

</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Example-1:-Postive-and-Negatives-Procedure">Example 1: Postive and Negatives Procedure<a class="anchor-link" href="#Example-1:-Postive-and-Negatives-Procedure"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="kd">function</span> <span class="nx">plusMinus</span><span class="p">(</span><span class="nx">arr</span><span class="p">)</span> <span class="p">{</span>
    <span class="kd">var</span> <span class="nx">pos</span> <span class="o">=</span> <span class="mf">0</span><span class="p">;</span>
    <span class="kd">var</span> <span class="nx">neg</span> <span class="o">=</span> <span class="mf">0</span><span class="p">;</span>
    <span class="kd">var</span> <span class="nx">zero</span> <span class="o">=</span> <span class="mf">0</span><span class="p">;</span>
    
    <span class="kd">var</span> <span class="nx">length</span> <span class="o">=</span> <span class="nx">arr</span><span class="p">.</span><span class="nx">length</span><span class="p">;</span>
    <span class="k">for</span> <span class="p">(</span><span class="kd">var</span> <span class="nx">i</span> <span class="o">=</span> <span class="mf">0</span><span class="p">;</span> <span class="nx">i</span> <span class="o">&lt;</span> <span class="nx">arr</span><span class="p">.</span><span class="nx">length</span><span class="p">;</span> <span class="nx">i</span><span class="o">++</span><span class="p">)</span> <span class="p">{</span>
        <span class="k">if</span> <span class="p">(</span><span class="nx">arr</span><span class="p">[</span><span class="nx">i</span><span class="p">]</span> <span class="o">&gt;</span> <span class="mf">0</span><span class="p">)</span> <span class="p">{</span>
          <span class="nx">pos</span> <span class="o">+=</span> <span class="mf">1</span><span class="p">;</span>
        <span class="p">}</span> <span class="k">else</span> <span class="k">if</span> <span class="p">(</span><span class="nx">arr</span><span class="p">[</span><span class="nx">i</span><span class="p">]</span> <span class="o">&lt;</span> <span class="mf">0</span><span class="p">)</span> <span class="p">{</span>
          <span class="nx">neg</span> <span class="o">+=</span> <span class="mf">1</span><span class="p">;</span>
        <span class="p">}</span> <span class="k">else</span> <span class="p">{</span>
          <span class="nx">zero</span> <span class="o">+=</span> <span class="mf">1</span><span class="p">;</span>
        <span class="p">}</span>
      <span class="p">}</span>
     <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;There are &quot;</span> <span class="o">+</span> <span class="nx">arr</span><span class="p">.</span><span class="nx">length</span> <span class="o">+</span> <span class="s2">&quot; total numbers&quot;</span><span class="p">);</span>
     <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;There are &quot;</span> <span class="o">+</span> <span class="nx">pos</span> <span class="o">+</span> <span class="s2">&quot; positive numbers&quot;</span><span class="p">);</span>
     <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;There are &quot;</span> <span class="o">+</span> <span class="nx">neg</span> <span class="o">+</span> <span class="s2">&quot; negative numbers&quot;</span><span class="p">);</span>
     <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;There are &quot;</span> <span class="o">+</span> <span class="nx">zero</span> <span class="o">+</span> <span class="s2">&quot; zeroes&quot;</span><span class="p">);</span>
    <span class="p">}</span>

    <span class="kd">var</span> <span class="nx">array</span> <span class="o">=</span> <span class="p">[</span><span class="mf">1</span><span class="p">,</span> <span class="mf">1</span><span class="p">,</span> <span class="mf">0</span> <span class="p">,</span> <span class="o">-</span><span class="mf">1</span><span class="p">,</span> <span class="o">-</span><span class="mf">1</span><span class="p">];</span>
    <span class="nx">plusMinus</span><span class="p">(</span><span class="nx">array</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>There are 5 total numbers
There are 2 positive numbers
There are 2 negative numbers
There are 1 zeroes
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Example-2:-Time-Conversion-Procedure">Example 2: Time Conversion Procedure<a class="anchor-link" href="#Example-2:-Time-Conversion-Procedure"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="kd">function</span> <span class="nx">timeConversion</span><span class="p">(</span><span class="nx">s</span><span class="p">)</span> <span class="p">{</span>
  <span class="kd">var</span> <span class="nx">arr</span> <span class="o">=</span> <span class="nx">s</span><span class="p">.</span><span class="nx">slice</span><span class="p">(</span><span class="mf">0</span><span class="p">,</span><span class="mf">8</span><span class="p">).</span><span class="nx">split</span><span class="p">(</span><span class="s1">&#39;:&#39;</span><span class="p">);</span>
  <span class="nx">arr</span><span class="p">[</span><span class="mf">0</span><span class="p">]</span> <span class="o">=</span> <span class="p">(</span><span class="nx">s</span><span class="p">.</span><span class="nx">indexOf</span><span class="p">(</span><span class="s1">&#39;PM&#39;</span><span class="p">)</span> <span class="o">&gt;</span> <span class="o">-</span><span class="mf">1</span><span class="p">)</span> <span class="o">?</span>
           <span class="p">(</span><span class="nx">arr</span><span class="p">[</span><span class="mf">0</span><span class="p">]</span> <span class="o">==</span> <span class="mf">12</span> <span class="o">?</span> <span class="s1">&#39;12&#39;</span> <span class="o">:</span> <span class="nb">Number</span><span class="p">(</span><span class="nx">arr</span><span class="p">[</span><span class="mf">0</span><span class="p">])</span> <span class="o">+</span> <span class="mf">12</span><span class="p">)</span> <span class="o">:</span>
           <span class="p">(</span><span class="nx">arr</span><span class="p">[</span><span class="mf">0</span><span class="p">]</span> <span class="o">==</span> <span class="mf">12</span> <span class="o">?</span> <span class="s1">&#39;00&#39;</span> <span class="o">:</span> <span class="nx">arr</span><span class="p">[</span><span class="mf">0</span><span class="p">]);</span>
  <span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">arr</span><span class="p">.</span><span class="nx">join</span><span class="p">(</span><span class="s1">&#39;:&#39;</span><span class="p">));</span>
  <span class="p">}</span>

  <span class="kd">var</span> <span class="nx">input</span> <span class="o">=</span> <span class="s2">&quot;07:05:45PM&quot;</span><span class="p">;</span>
  <span class="nx">timeConversion</span><span class="p">(</span><span class="nx">input</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>19:05:45
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Challenge-2:-Min-and-Max-(Bonus-0.1-points):-You-can-do-this-whole-thing-in-either-Python-or-JavaScript."><mark>Challenge 2</mark>: Min and Max (Bonus 0.1 points): You can do this whole thing in either Python or JavaScript.<a class="anchor-link" href="#Challenge-2:-Min-and-Max-(Bonus-0.1-points):-You-can-do-this-whole-thing-in-either-Python-or-JavaScript."> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="c1">// Start by creating a procedure called findMax and set the parameters to numberA and numberB.</span>

<span class="c1">// Within the procedure, write the code to determine which of the two parameters, numberA or numberB, is the larger value. Print that value.</span>

<span class="c1">// Repeat the process, this time creating a procedure called findMin, which will print the parameter with a smaller value.</span>

<span class="c1">// Call both functions so that the parameters numberA and numberB are given a value.</span>

<span class="c1">// Optional bonus- create a procedure that can determine the minimum or maximum value out of more than two parameters.</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

</div>
 

