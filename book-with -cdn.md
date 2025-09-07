<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Programming Book with Colorful Syntax</title>
    <style>
/* === BASE === */
body {
    font-family: "Fira Sans", "Source Sans Pro", "DejaVu Sans", sans-serif;
    line-height: 1.7;
    margin: 2em;
    background: #fafafa;
    color: #2d3748;
}

/* Headers */
h1, h2, h3, h4 {
    font-family: "Fira Sans", "Roboto", sans-serif;
    font-weight: 700;
    margin-top: 2em;
    margin-bottom: 0.8em;
}
h1 { color: #e53e3e; font-size: 2.5em; border-bottom: 3px solid #e53e3e; padding-bottom: 0.3em; }
h2 { color: #dd6b20; font-size: 2em; }
h3 { color: #d69e2e; font-size: 1.5em; }
h4 { color: #38a169; font-size: 1.2em; }

/* Code blocks */
pre {
    background: linear-gradient(135deg, #1a202c 0%, #2d3748 100%);
    color: #f7fafc;
    padding: 1.5em;
    border-radius: 12px;
    overflow-x: auto;
    font-size: 0.95em;
    font-family: "Fira Code", "JetBrains Mono", monospace;
    border: 1px solid #4a5568;
    box-shadow: 0 8px 25px rgba(0,0,0,0.15);
    position: relative;
    margin: 1.5em 0;
}
pre::before {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: linear-gradient(90deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4, #ffeaa7);
    border-radius: 12px 12px 0 0;
}

/* Inline code */
code {
    background: linear-gradient(135deg, #4a5568, #2d3748);
    color: #ffd700;
    padding: 3px 6px;
    border-radius: 6px;
    font-family: "Fira Code", monospace;
    font-size: 0.9em;
    border: 1px solid #718096;
}

/* Syntax highlighting */
.hljs-keyword, .hljs-selector-tag, .hljs-literal { color: #82aaff !important; font-weight: bold; }
.hljs-type, .hljs-class { color: #4dd0e1 !important; font-weight: 600; }
.hljs-string { color: #c3e88d !important; }
.hljs-number { color: #ffcb6b !important; font-weight: 600; }
.hljs-comment { color: #546e7a !important; font-style: italic; opacity: 0.8; }
.hljs-function, .hljs-title.function { color: #c792ea !important; font-weight: 600; }
.hljs-variable, .hljs-property { color: #89ddff !important; }
.hljs-operator { color: #ff5370 !important; font-weight: 600; }
.hljs-built_in { color: #ffcb6b !important; font-weight: 600; }
.hljs-meta, .hljs-tag { color: #f78c6c !important; }
.hljs-params { color: #ffab91 !important; }

/* Badges */
pre[class*="language-"]::after {
    position: absolute;
    top: 0.3em;
    right: 1em;
    padding: 0.2em 0.6em;
    font-size: 0.75em;
    font-weight: bold;
    border-radius: 4px;
    opacity: 0.8;
    color: white;
}
pre.language-kotlin::after { content: "Kotlin"; background: #7c4dff; }
pre.language-php::after { content: "PHP"; background: #8e44ad; }
pre.language-sql::after { content: "SQL"; background: #e74c3c; }
pre.language-python::after { content: "Python"; background: #3498db; }
pre.language-javascript::after { content: "JavaScript"; background: #f1c40f; color: #2c3e50; }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/default.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
    <script>hljs.highlightAll();</script>
</head>
<body>

<h1>Livre de Démonstration – Pandoc + Code Highlighting</h1>
<p>Bienvenue dans ce livre de test avec <strong>Pandoc</strong> et Highlight.js 🎨.</p>

<hr>

<h2>Chapitre 1 – Kotlin</h2>
<pre><code class="language-kotlin">class Person(val name: String, val age: Int) {
    fun greet() {
        println("Bonjour, je m'appelle $name et j'ai $age ans.")
    }
}

fun main() {
    val p = Person("Ali", 25)
    p.greet()
}</code></pre>

<h2>Chapitre 2 – PHP</h2>
<pre><code class="language-php">&lt;?php
class Person {
    public $name;
    public $age;

    function __construct($name, $age) {
        $this->name = $name;
        $this->age = $age;
    }

    function greet() {
        echo "Bonjour, je m'appelle {$this->name} et j'ai {$this->age} ans.";
    }
}

$p = new Person("Ali", 25);
$p->greet();
?&gt;</code></pre>

<h2>Chapitre 3 – SQL</h2>
<pre><code class="language-sql">CREATE TABLE persons (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(50),
    age INT
);

INSERT INTO persons (name, age) VALUES ('Ali', 25);
SELECT * FROM persons;</code></pre>

<h2>Chapitre 4 – Python</h2>
<pre><code class="language-python">class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print(f"Bonjour, je m'appelle {self.name} et j'ai {self.age} ans.")

p = Person("Ali", 25)
p.greet()</code></pre>

<h2>Chapitre 5 – JavaScript</h2>
<pre><code class="language-javascript">class Person {
    constructor(name, age) {
        this.name = name;
        this.age = age;
    }

    greet() {
        console.log(`Bonjour, je m'appelle ${this.name} et j'ai ${this.age} ans.`);
    }
}

const p = new Person("Ali", 25);
p.greet();</code></pre>

</body>
</html>
