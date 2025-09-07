<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apprendre Kotlin - Programming Book</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<h1>Livre de Démonstration – Pandoc + Code Highlighting</h1>

<p>Bienvenue dans ce livre de test.<br>
L'objectif est de vérifier la mise en forme avec <strong>Pandoc</strong>.</p>

<hr>

<h2>Chapitre 1 – Kotlin</h2>

<div class="sourceCode" id="cb1"><pre class="sourceCode kotlin"><code class="sourceCode kotlin">
<span class="kw">class</span> <span class="dt">Person</span>(<span class="kw">val</span> name: <span class="dt">String</span>, <span class="kw">val</span> age: <span class="dt">Int</span>) {
    <span class="kw">fun</span> <span class="fu">greet</span>() {
        <span class="fu">println</span>(<span class="st">"Bonjour, je m'appelle </span><span class="sc">$name</span><span class="st"> et j'ai </span><span class="sc">$age</span><span class="st"> ans."</span>)
    }
}

<span class="kw">fun</span> <span class="fu">main</span>() {
    <span class="kw">val</span> p = <span class="fu">Person</span>(<span class="st">"Ali"</span>, <span class="dv">25</span>)
    p.<span class="fu">greet</span>()
}
</code></pre></div>

<h2>Chapitre 2 – PHP</h2>

<div class="sourceCode" id="cb2"><pre class="sourceCode php"><code class="sourceCode php">
<span class="kw">&lt;?php</span>
<span class="kw">class</span> Person {
    <span class="kw">public</span> <span class="va">$name</span>;
    <span class="kw">public</span> <span class="va">$age</span>;

    <span class="kw">function</span> <span class="fu">__construct</span>(<span class="va">$name</span>, <span class="va">$age</span>) {
        <span class="va">$this</span>-&gt;name = <span class="va">$name</span>;
        <span class="va">$this</span>-&gt;age = <span class="va">$age</span>;
    }

    <span class="kw">function</span> <span class="fu">greet</span>() {
        <span class="kw">echo</span> <span class="st">"Bonjour, je m'appelle {</span><span class="va">$this</span><span class="st">-&gt;name} et j'ai {</span><span class="va">$this</span><span class="st">-&gt;age} ans."</span>;
    }
}

<span class="va">$p</span> = <span class="kw">new</span> Person(<span class="st">"Ali"</span>, <span class="dv">25</span>);
<span class="va">$p</span>-&gt;<span class="fu">greet</span>();
<span class="kw">?&gt;</span>
</code></pre></div>

<h2>Chapitre 3 – SQL</h2>

<div class="sourceCode" id="cb3"><pre class="sourceCode sql"><code class="sourceCode sql">
<span class="kw">CREATE</span> <span class="kw">TABLE</span> persons (
    id <span class="dt">INT</span> <span class="kw">PRIMARY</span> <span class="kw">KEY</span> <span class="kw">AUTO_INCREMENT</span>,
    name <span class="dt">VARCHAR</span>(<span class="dv">50</span>),
    age <span class="dt">INT</span>
);

<span class="kw">INSERT</span> <span class="kw">INTO</span> persons (name, age) <span class="kw">VALUES</span> (<span class="st">'Ali'</span>, <span class="dv">25</span>);

<span class="kw">SELECT</span> <span class="op">*</span> <span class="kw">FROM</span> persons;
</code></pre></div>

<h2>Chapitre 4 – Python</h2>

<div class="sourceCode" id="cb4"><pre class="sourceCode python"><code class="sourceCode python">
<span class="kw">class</span> Person:
    <span class="kw">def</span> <span class="fu">__init__</span>(<span class="va">self</span>, name, age):
        <span class="va">self</span>.name <span class="op">=</span> name
        <span class="va">self</span>.age <span class="op">=</span> age

    <span class="kw">def</span> <span class="fu">greet</span>(<span class="va">self</span>):
        <span class="bu">print</span>(<span class="ss">f"Bonjour, je m'appelle </span><span class="sc">{</span><span class="va">self</span><span class="sc">.</span>name<span class="sc">}</span><span class="ss"> et j'ai </span><span class="sc">{</span><span class="va">self</span><span class="sc">.</span>age<span class="sc">}</span><span class="ss"> ans."</span>)

p <span class="op">=</span> Person(<span class="st">"Ali"</span>, <span class="dv">25</span>)
p.greet()
</code></pre></div>

<h2>Chapitre 5 – JavaScript</h2>

<div class="sourceCode" id="cb5"><pre class="sourceCode javascript"><code class="sourceCode javascript">
<span class="kw">class</span> Person {
    <span class="fu">constructor</span>(name<span class="op">,</span> age) {
        <span class="kw">this</span><span class="op">.</span><span class="at">name</span> <span class="op">=</span> name<span class="op">;</span>
        <span class="kw">this</span><span class="op">.</span><span class="at">age</span> <span class="op">=</span> age<span class="op">;</span>
    }

    <span class="fu">greet</span>() {
        <span class="bu">console</span><span class="op">.</span><span class="fu">log</span>(<span class="vs">`Bonjour, je m'appelle </span><span class="sc">${</span><span class="kw">this</span><span class="sc">.</span><span class="at">name</span><span class="sc">}</span><span class="vs"> et j'ai </span><span class="sc">${</span><span class="kw">this</span><span class="sc">.</span><span class="at">age</span><span class="sc">}</span><span class="vs"> ans.`</span>)<span class="op">;</span>
    }
}

<span class="kw">const</span> p <span class="op">=</span> <span class="kw">new</span> Person(<span class="st">"Ali"</span><span class="op">,</span> <span class="dv">25</span>)<span class="op">;</span>
p<span class="op">.</span><span class="fu">greet</span>()<span class="op">;</span>
</code></pre></div>

</body>
</html>