---


---

<h1 id="react">React</h1>
<h2 id="getting-started">Getting Started</h2>
<ul>
<li>react is library for web/native user interfaces.</li>
</ul>
<h4 id="there-are-different-way-to-create-react-app.">There are different way to create react app.</h4>
<ol>
<li>Quick way - React.new - in browser.</li>
<li>Local React project:- vite, reactapp
<ol start="3">
<li>Vite -&gt;</li>
</ol>
</li>
</ol>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">npm</span> i/install
<span class="token comment"># cd -&gt;</span>
<span class="token function">npm</span> run dev
</code></pre>
<ol start="3">
<li>HTML + JS = JSX - which cannot directly render in to the browser.</li>
</ol>
<h4 id="vite-commands">Vite commands:</h4>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">npm</span> create vite@Latest <span class="token punctuation">[</span>project-name<span class="token punctuation">]</span>
<span class="token function">cd</span> <span class="token punctuation">[</span>project-name<span class="token punctuation">]</span>
<span class="token function">npm</span> <span class="token function">install</span>
<span class="token function">npm</span> run dev
</code></pre>
<hr>
<h1 id="javascript-refresher">JavaScript Refresher</h1>
<ul>
<li>JS can be run via (Browser, [node.js, demo], [Capacitor, React Native])</li>
<li>can include <code>&lt;script src="[filename].js"&gt;&lt;/script&gt;</code></li>
</ul>
<pre class=" language-html"><code class="prism  language-html"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>script</span> <span class="token attr-name">defer</span><span class="token punctuation">&gt;</span></span><span class="token script language-javascript"></span><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>script</span><span class="token punctuation">&gt;</span></span> 
# used to ensure run script after HTML element loaded
</code></pre>
<pre class=" language-html"><code class="prism  language-html"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>script</span> <span class="token attr-name">type</span><span class="token attr-value"><span class="token punctuation">=</span><span class="token punctuation">"</span>module<span class="token punctuation">"</span></span><span class="token punctuation">&gt;</span></span><span class="token script language-javascript"></span><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>script</span><span class="token punctuation">&gt;</span></span> 
# it enables import export
</code></pre>
<pre class=" language-html"><code class="prism  language-html"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>noscript</span><span class="token punctuation">&gt;</span></span><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>script</span><span class="token punctuation">&gt;</span></span> 
# it shows when user runs without js.
</code></pre>
<ul>
<li>usually react build JS and inject in browser as script.</li>
<li>JSX is not JS default feature.</li>
</ul>
<h4 id="import--export">import &amp; export</h4>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">export</span> <span class="token keyword">let</span> <span class="token keyword">var</span><span class="token operator">-</span>name <span class="token operator">=</span> <span class="token string">"value"</span><span class="token punctuation">;</span>
<span class="token keyword">import</span> <span class="token punctuation">{</span> <span class="token keyword">var</span><span class="token operator">-</span>name<span class="token punctuation">,</span><span class="token punctuation">[</span><span class="token punctuation">,</span><span class="token punctuation">,</span><span class="token operator">...</span><span class="token punctuation">.</span><span class="token punctuation">]</span> <span class="token punctuation">}</span> form <span class="token string">"./file-name.js"</span><span class="token punctuation">;</span>
# js <span class="token keyword">in</span> <span class="token operator">/</span> but <span class="token keyword">in</span> react there is no extention
</code></pre>
<ul>
<li>need to use the script as type module.(in vanilla JavaScript)</li>
</ul>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">export</span> <span class="token keyword">default</span> <span class="token string">"value"</span><span class="token punctuation">;</span>
# must only one <span class="token keyword">default</span>
<span class="token keyword">import</span> <span class="token keyword">var</span><span class="token operator">-</span>name <span class="token keyword">from</span> <span class="token string">"./file-name.js"</span><span class="token punctuation">;</span>
</code></pre>
<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token keyword">import</span> <span class="token operator">*</span> <span class="token keyword">as</span> <span class="token keyword">var</span><span class="token operator">-</span>name <span class="token keyword">from</span> <span class="token string">"./file-name.js"</span><span class="token punctuation">;</span>
# the <span class="token keyword">var</span><span class="token operator">-</span>name become js object
<span class="token keyword">import</span> <span class="token punctuation">{</span><span class="token keyword">var</span><span class="token operator">-</span>name1<span class="token punctuation">,</span> <span class="token keyword">var</span><span class="token operator">-</span><span class="token keyword">in</span><span class="token operator">-</span>file <span class="token keyword">as</span> name<span class="token operator">-</span>u<span class="token operator">-</span>want<span class="token punctuation">}</span> <span class="token keyword">from</span> file<span class="token operator">-</span>name<span class="token punctuation">;</span>
</code></pre>
<h4 id="variable-values">Variable, values</h4>
<pre><code>let || const
</code></pre>
<h4 id="operator">Operator</h4>
<pre><code>+ _ * /
&lt; &gt; == === &lt;= &gt;=
</code></pre>
<h4 id="functions">Functions</h4>
<pre class=" language-js"><code class="prism  language-js"><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span><span class="token punctuation">}</span>
</code></pre>
<p>or</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">function</span> <span class="token function">f_name</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">{</span>
	<span class="token keyword">return</span> <span class="token string">'value'</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span>
</code></pre>
<h4 id="class">Class</h4>
<ul>
<li>Class name should start with capital letter</li>
</ul>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">class</span> <span class="token class-name">ClassName</span> <span class="token punctuation">{</span>
  <span class="token function">constructor</span><span class="token punctuation">(</span>parameter1<span class="token punctuation">,</span> parameter2<span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token keyword">this</span><span class="token punctuation">.</span>property1 <span class="token operator">=</span> parameter1<span class="token punctuation">;</span>
    <span class="token keyword">this</span><span class="token punctuation">.</span>property2 <span class="token operator">=</span> parameter2<span class="token punctuation">;</span>
  <span class="token punctuation">}</span>

  <span class="token function">methodName</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span><span class="token comment">/* code for method */</span><span class="token punctuation">}</span>
<span class="token punctuation">}</span>
</code></pre>
<p>Or object literal</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> person <span class="token operator">=</span> <span class="token punctuation">{</span>
  name<span class="token punctuation">:</span> <span class="token string">"John"</span><span class="token punctuation">,</span>
  age<span class="token punctuation">:</span> <span class="token number">25</span><span class="token punctuation">,</span>
  greet<span class="token punctuation">:</span> <span class="token keyword">function</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"name"</span> <span class="token operator">+</span> <span class="token keyword">this</span><span class="token punctuation">.</span>name<span class="token punctuation">)</span><span class="token punctuation">;</span>
  <span class="token punctuation">}</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>
</code></pre>
<h4 id="arrays">Arrays</h4>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> arr <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
fruits<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span><span class="token number">4</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token keyword">const</span> index <span class="token operator">=</span> numbers<span class="token punctuation">.</span><span class="token function">findIndex</span><span class="token punctuation">(</span>num <span class="token operator">=&gt;</span> num <span class="token operator">&gt;</span> <span class="token number">2</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token keyword">const</span> doubled <span class="token operator">=</span> nums<span class="token punctuation">.</span><span class="token function">map</span><span class="token punctuation">(</span>n <span class="token operator">=&gt;</span> n <span class="token operator">*</span> <span class="token number">2</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<h4 id="destructuring-array">Destructuring Array</h4>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> <span class="token punctuation">[</span>a<span class="token punctuation">,</span> b<span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
<span class="token keyword">const</span> <span class="token punctuation">[</span>x<span class="token punctuation">,</span> <span class="token punctuation">,</span> y<span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">]</span><span class="token punctuation">;</span>   <span class="token comment">// Skip</span>
<span class="token keyword">const</span> <span class="token punctuation">[</span>first<span class="token punctuation">,</span> <span class="token operator">...</span>rest<span class="token punctuation">]</span> <span class="token operator">=</span> arr<span class="token punctuation">;</span>
<span class="token punctuation">[</span>a<span class="token punctuation">,</span> b<span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token punctuation">[</span>b<span class="token punctuation">,</span> a<span class="token punctuation">]</span><span class="token punctuation">;</span>              <span class="token comment">// Swap</span>
</code></pre>
<h4 id="spread-operation">Spread operation</h4>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> arr <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
<span class="token keyword">const</span> newArr <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token operator">...</span>arr<span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">]</span><span class="token punctuation">;</span>                  <span class="token comment">// → [1, 2, 3]</span>

<span class="token keyword">const</span> obj <span class="token operator">=</span> <span class="token punctuation">{</span> a<span class="token punctuation">:</span> <span class="token number">1</span> <span class="token punctuation">}</span><span class="token punctuation">;</span>
<span class="token keyword">const</span> newObj <span class="token operator">=</span> <span class="token punctuation">{</span> <span class="token operator">...</span>obj<span class="token punctuation">,</span> b<span class="token punctuation">:</span> <span class="token number">2</span> <span class="token punctuation">}</span><span class="token punctuation">;</span>             <span class="token comment">// → { a: 1, b: 2 }</span>

<span class="token keyword">const</span> nums <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">10</span><span class="token punctuation">,</span> <span class="token number">20</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
Math<span class="token punctuation">.</span><span class="token function">max</span><span class="token punctuation">(</span><span class="token operator">...</span>nums<span class="token punctuation">)</span><span class="token punctuation">;</span>                           <span class="token comment">// → 20</span>
</code></pre>

