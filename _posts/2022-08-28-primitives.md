---
keywords: fastai
description: a primitives demo
title: Primitives Notebook
toc: true
badges: true
comments: true
categories: [fastpages, jupyter]
nb_path: _notebooks/2022-08-28-primitives.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-28-primitives.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Listing-the-types-of-primitives:">Listing the types of primitives:<a class="anchor-link" href="#Listing-the-types-of-primitives:"> </a></h3>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="kd">public</span> <span class="kd">class</span> <span class="nc">ListPrimitives</span> <span class="p">{</span>
    <span class="kd">public</span> <span class="kd">static</span> <span class="kt">void</span> <span class="nf">main</span><span class="p">(</span><span class="n">String</span><span class="o">[]</span> <span class="n">args</span><span class="p">)</span> <span class="p">{</span>
      
      <span class="c1">// assigning variable values</span>
      <span class="kt">int</span> <span class="n">anInt</span> <span class="o">=</span> <span class="mi">505</span><span class="p">;</span>
      <span class="kt">double</span> <span class="n">aDouble</span> <span class="o">=</span> <span class="mf">99.9</span><span class="p">;</span>
      <span class="kt">boolean</span> <span class="n">aBoolean</span> <span class="o">=</span> <span class="kc">true</span><span class="p">;</span>
      <span class="kt">char</span> <span class="n">aChar</span><span class="o">=</span><span class="sc">&#39;\u0021&#39;</span><span class="p">;</span>  
      <span class="c1">// not a primitive but essential</span>
      <span class="n">String</span> <span class="n">aString</span> <span class="o">=</span> <span class="s">&quot;Look over there!&quot;</span><span class="p">;</span>
  
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Types of Primitives:&quot;</span><span class="p">);</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;--&gt; Integer: &quot;</span> <span class="o">+</span> <span class="n">anInt</span><span class="p">);</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;--&gt; Double: &quot;</span> <span class="o">+</span> <span class="n">aDouble</span><span class="p">);</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;--&gt; Character: &quot;</span> <span class="o">+</span> <span class="n">aChar</span><span class="p">);</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;--&gt; Boolean: &quot;</span> <span class="o">+</span> <span class="n">aBoolean</span><span class="p">);</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;--&gt; String: &quot;</span> <span class="o">+</span> <span class="n">aString</span><span class="p">);</span>
    <span class="p">}</span>
  <span class="p">}</span>
  <span class="n">ListPrimitives</span><span class="p">.</span><span class="na">main</span><span class="p">(</span><span class="kc">null</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Types of Primitives:
--&gt; Integer: 505
--&gt; Double: 99.9
--&gt; Character: !
--&gt; Boolean: true
--&gt; String: Look over there!
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Division-with-ints-and-doubles:">Division with ints and doubles:<a class="anchor-link" href="#Division-with-ints-and-doubles:"> </a></h3>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="kd">public</span> <span class="kd">class</span> <span class="nc">Division</span> <span class="p">{</span>
    <span class="kd">public</span> <span class="kd">static</span> <span class="kt">void</span> <span class="nf">main</span><span class="p">(</span><span class="n">String</span><span class="o">[]</span> <span class="n">args</span><span class="p">)</span> <span class="p">{</span>
  
      <span class="c1">// setting the variables</span>
      <span class="kt">int</span> <span class="n">divided</span> <span class="o">=</span> <span class="mi">17</span> <span class="o">/</span> <span class="mi">24</span><span class="p">;</span>
      <span class="kt">double</span> <span class="n">doubleDivided</span> <span class="o">=</span> <span class="mf">17.0</span> <span class="o">/</span> <span class="mf">24.0</span><span class="p">;</span>
  
      <span class="c1">// printing out the division in int and double form</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Integer division with 17/24 is: &quot;</span> <span class="o">+</span> <span class="n">divided</span><span class="p">);</span>
      <span class="c1">// %.2f limits the # of decimal values displayed</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Double division with 17.0/24.0 is: &quot;</span> <span class="o">+</span> <span class="n">String</span><span class="p">.</span><span class="na">format</span><span class="p">(</span><span class="s">&quot;%.2f&quot;</span><span class="p">,</span> <span class="n">doubleDivided</span><span class="p">));</span>      
    <span class="p">}</span>
  <span class="p">}</span>
  <span class="c1">// makes it so you can print the code&#39;s output</span>
  <span class="n">Division</span><span class="p">.</span><span class="na">main</span><span class="p">(</span><span class="kc">null</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Integer division with 17/24 is: 0
Double division with 17.0/24.0 is: 0.71
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Celsius-to-Fahrenheit-Converter">Celsius to Fahrenheit Converter<a class="anchor-link" href="#Celsius-to-Fahrenheit-Converter"> </a></h3>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="kd">public</span> <span class="kd">class</span> <span class="nc">CtoF</span> <span class="p">{</span>
    <span class="kd">public</span> <span class="kd">static</span> <span class="kt">void</span> <span class="nf">main</span><span class="p">(</span><span class="n">String</span><span class="o">[]</span> <span class="n">args</span><span class="p">)</span> <span class="p">{</span>
  
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Celsius to Fahrenheit Converter:&quot;</span><span class="p">);</span>

      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Degrees Celsius: 55 --&gt;&quot;</span><span class="p">);</span>
      <span class="kt">int</span> <span class="n">celsius</span> <span class="o">=</span> <span class="mi">55</span><span class="p">;</span>
      <span class="kt">int</span> <span class="n">fahrenheit</span> <span class="o">=</span> <span class="p">((</span><span class="n">celsius</span><span class="o">*</span><span class="mi">9</span><span class="p">)</span><span class="o">/</span><span class="mi">5</span><span class="p">)</span><span class="o">+</span><span class="mi">32</span><span class="p">;</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;\tDegrees Fahrenheit: &quot;</span> <span class="o">+</span> <span class="n">fahrenheit</span><span class="p">);</span>

      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Degrees Celsius: 78 --&gt;&quot;</span><span class="p">);</span>
      <span class="kt">int</span> <span class="n">celsius1</span> <span class="o">=</span> <span class="mi">78</span><span class="p">;</span>
      <span class="kt">int</span> <span class="n">fahrenheit1</span> <span class="o">=</span> <span class="p">((</span><span class="n">celsius1</span><span class="o">*</span><span class="mi">9</span><span class="p">)</span><span class="o">/</span><span class="mi">5</span><span class="p">)</span><span class="o">+</span><span class="mi">32</span><span class="p">;</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;\tDegrees Fahrenheit: &quot;</span> <span class="o">+</span> <span class="n">fahrenheit1</span><span class="p">);</span>

      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Degrees Celsius: 11 --&gt;&quot;</span><span class="p">);</span>
      <span class="kt">int</span> <span class="n">celsius2</span> <span class="o">=</span> <span class="mi">11</span><span class="p">;</span>
      <span class="kt">int</span> <span class="n">fahrenheit2</span> <span class="o">=</span> <span class="p">((</span><span class="n">celsius2</span><span class="o">*</span><span class="mi">9</span><span class="p">)</span><span class="o">/</span><span class="mi">5</span><span class="p">)</span><span class="o">+</span><span class="mi">32</span><span class="p">;</span>
      <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;\tDegrees Fahrenheit: &quot;</span> <span class="o">+</span> <span class="n">fahrenheit2</span><span class="p">);</span>
    
    <span class="p">}</span>
  <span class="p">}</span>
  <span class="c1">// makes it so you can print the code&#39;s output</span>
  <span class="n">CtoF</span><span class="p">.</span><span class="na">main</span><span class="p">(</span><span class="kc">null</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Celsius to Fahrenheit Converter:
Degrees Celsius: 55 --&gt;
	Degrees Fahrenheit: 131
Degrees Celsius: 78 --&gt;
	Degrees Fahrenheit: 172
Degrees Celsius: 11 --&gt;
	Degrees Fahrenheit: 51
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Inputting-primitive-data:">Inputting primitive data:<a class="anchor-link" href="#Inputting-primitive-data:"> </a></h3>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="c1">// java style to import library</span>
<span class="kn">import</span> <span class="nn">java.util.Scanner</span><span class="p">;</span>

<span class="c1">// class must alway have 1st letter as uppercase, CamelCase is Java Class convention</span>
<span class="kd">public</span> <span class="kd">class</span> <span class="nc">ScanPrimitives</span> <span class="p">{</span>
    <span class="kd">public</span> <span class="kd">static</span> <span class="kt">void</span> <span class="nf">main</span><span class="p">(</span><span class="n">String</span><span class="o">[]</span> <span class="n">args</span><span class="p">)</span> <span class="p">{</span>    
        <span class="n">Scanner</span> <span class="n">input</span><span class="p">;</span>

        <span class="c1">// primitive int</span>
        <span class="n">input</span> <span class="o">=</span> <span class="k">new</span> <span class="n">Scanner</span><span class="p">(</span><span class="n">System</span><span class="p">.</span><span class="na">in</span><span class="p">);</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">print</span><span class="p">(</span><span class="s">&quot;Enter an integer: &quot;</span><span class="p">);</span>
        <span class="k">try</span> <span class="p">{</span>
            <span class="kt">int</span> <span class="n">sampleInputInt</span> <span class="o">=</span> <span class="n">input</span><span class="p">.</span><span class="na">nextInt</span><span class="p">();</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">sampleInputInt</span><span class="p">);</span>
        <span class="p">}</span> <span class="k">catch</span> <span class="p">(</span><span class="n">Exception</span> <span class="n">e</span><span class="p">)</span> <span class="p">{</span>  <span class="c1">// if not an integer</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Not an integer (form like 159), &quot;</span> <span class="o">+</span> <span class="n">e</span><span class="p">);</span>
        <span class="p">}</span>
        <span class="n">input</span><span class="p">.</span><span class="na">close</span><span class="p">();</span>

        <span class="c1">// primitive double</span>
        <span class="n">input</span> <span class="o">=</span> <span class="k">new</span> <span class="n">Scanner</span><span class="p">(</span><span class="n">System</span><span class="p">.</span><span class="na">in</span><span class="p">);</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">print</span><span class="p">(</span><span class="s">&quot;Enter a double: &quot;</span><span class="p">);</span>
        <span class="k">try</span> <span class="p">{</span>
            <span class="kt">double</span> <span class="n">sampleInputDouble</span> <span class="o">=</span> <span class="n">input</span><span class="p">.</span><span class="na">nextDouble</span><span class="p">();</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">sampleInputDouble</span><span class="p">);</span>
        <span class="p">}</span> <span class="k">catch</span> <span class="p">(</span><span class="n">Exception</span> <span class="n">e</span><span class="p">)</span> <span class="p">{</span>  <span class="c1">// if not a number</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Not an double (form like 9.99), &quot;</span> <span class="o">+</span> <span class="n">e</span><span class="p">);</span>
        <span class="p">}</span>
        <span class="n">input</span><span class="p">.</span><span class="na">close</span><span class="p">();</span>

        <span class="c1">// primitive boolean</span>
        <span class="n">input</span> <span class="o">=</span>  <span class="k">new</span> <span class="n">Scanner</span><span class="p">(</span><span class="n">System</span><span class="p">.</span><span class="na">in</span><span class="p">);</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">print</span><span class="p">(</span><span class="s">&quot;Enter a boolean: &quot;</span><span class="p">);</span>
        <span class="k">try</span> <span class="p">{</span>
            <span class="kt">boolean</span> <span class="n">sampleInputBoolean</span> <span class="o">=</span> <span class="n">input</span><span class="p">.</span><span class="na">nextBoolean</span><span class="p">();</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">sampleInputBoolean</span><span class="p">);</span>
        <span class="p">}</span> <span class="k">catch</span> <span class="p">(</span><span class="n">Exception</span> <span class="n">e</span><span class="p">)</span> <span class="p">{</span>  <span class="c1">// if not true or false</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Not an boolean (true or false), &quot;</span> <span class="o">+</span> <span class="n">e</span><span class="p">);</span>
        <span class="p">}</span>
        <span class="n">input</span><span class="p">.</span><span class="na">close</span><span class="p">();</span>

        <span class="c1">// wrapper class String</span>
        <span class="n">input</span> <span class="o">=</span>  <span class="k">new</span> <span class="n">Scanner</span><span class="p">(</span><span class="n">System</span><span class="p">.</span><span class="na">in</span><span class="p">);</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">print</span><span class="p">(</span><span class="s">&quot;Enter a String: &quot;</span><span class="p">);</span>
        <span class="k">try</span> <span class="p">{</span>
            <span class="n">String</span> <span class="n">sampleInputString</span> <span class="o">=</span> <span class="n">input</span><span class="p">.</span><span class="na">nextLine</span><span class="p">();</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">sampleInputString</span><span class="p">);</span>
        <span class="p">}</span> <span class="k">catch</span> <span class="p">(</span><span class="n">Exception</span> <span class="n">e</span><span class="p">)</span> <span class="p">{</span> <span class="c1">// this may never happen</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Not an String, &quot;</span> <span class="o">+</span> <span class="n">e</span><span class="p">);</span>
        <span class="p">}</span>
        <span class="n">input</span><span class="p">.</span><span class="na">close</span><span class="p">();</span>
    <span class="p">}</span>
<span class="p">}</span>
<span class="n">ScanPrimitives</span><span class="p">.</span><span class="na">main</span><span class="p">(</span><span class="kc">null</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Enter an integer: 2
Enter a double: 2.0
Enter a boolean: true
Enter a String: hi
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

