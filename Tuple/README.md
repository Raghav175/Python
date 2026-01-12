<h1 align="center">🐍 Python Tuples</h1>

<p align="center">
  <b>Ordered, immutable collections used for fixed, reliable data grouping</b>
</p>

<hr/>

<h2>📘 Overview</h2>

<li>
A <b>tuple</b> is an ordered sequence of items in Python, enclosed in
parentheses <code>( )</code> and separated by commas <code>,</code>.
</li>

<li>
Tuples can store <b>heterogeneous data types</b> (int, float, string, list, object, etc.)
within a single structure.
</li>

<li>
Once created, a tuple <b>cannot be modified in place</b>. Its memory layout is fixed,
so elements can <b>neither be added nor deleted</b>. Any operation that appears to
change a tuple actually creates a <b>new tuple object in memory</b>.
</li>

<li>
Tuples are commonly used to represent <b>fixed records</b>, <b>configuration values</b>,
and <b>multiple values returned from functions</b>.
</li>

---

<h2>🧬 Key Characteristics</h2>

<table>
  <tr>
    <th align="left">Property</th>
    <th align="left">Description</th>
  </tr>

  <tr>
    <td>Creation</td>
    <td>Parentheses <code>( )</code> with comma-separated values</td>
  </tr>

  <tr>
    <td>Mutability</td>
    <td><b>Immutable</b> (cannot be changed after creation)</td>
  </tr>

  <tr>
    <td>Order</td>
    <td>Maintains insertion order</td>
  </tr>

  <tr>
    <td>Indexing</td>
    <td>Supports zero-based and negative indexing</td>
  </tr>

  <tr>
    <td>Slicing</td>
    <td>Supported (returns a new tuple)</td>
  </tr>

  <tr>
    <td>Duplicates</td>
    <td>Allowed</td>
  </tr>
</table>

---

<h2>🧱 Immutability Explained</h2>

<p>Tuples do <b>not</b> support:</p>

<ul>
  <li>Item reassignment</li>
  <li>Insertion or deletion of elements</li>
</ul>

<p>
This immutability makes tuples:
</p>

<ul>
  <li>Safer for shared data</li>
  <li>Hashable (usable as dictionary keys if elements are immutable)</li>
  <li>More memory-efficient than lists</li>
</ul>

---

<h2>🔍 Accessing Elements</h2>

<ul>
  <li>Index-based access: <code>t[0]</code></li>
  <li>Negative indexing: <code>t[-1]</code></li>
  <li>Slicing: <code>t[1:4]</code></li>
  <li>Step slicing: <code>t[::2]</code></li>
</ul>

<p>
<b>Important:</b> Slicing always produces a <b>new tuple</b>.
</p>

---

<h2>🛠 Common Tuple Methods</h2>

<pre>
.index()
.count()
</pre>

<p>
Tuples expose very few methods by design, reinforcing their role as
<b>read-only data containers</b>.
</p>

---

<h2>📦 Tuple Packing</h2>

<p>
<b>Packing</b> means grouping multiple values into a single tuple automatically.
</p>

<pre>
data = 10, 20, 30
</pre>

<p>
Parentheses are optional; commas do the real work.
</p>

<p><b>Why packing exists:</b></p>

<ul>
  <li>Clean grouping of related values</li>
  <li>Efficient return of multiple values from functions</li>
  <li>Improved code readability</li>
</ul>

---

<h2>📤 Tuple Unpacking</h2>

<p>
<b>Unpacking</b> extracts tuple elements into individual variables.
</p>

<pre>
x, y, z = data
</pre>

<p><b>Why unpacking exists:</b></p>

<ul>
  <li>Eliminates index-based access</li>
  <li>Makes intent explicit</li>
  <li>Reduces boilerplate code</li>
</ul>

<p>
Python enforces <b>exact positional matching</b> during unpacking unless using extended unpacking.
</p>

---

<h2>⭐ Extended Unpacking</h2>

<pre>
a, *b, c = (1, 2, 3, 4, 5)
</pre>

<ul>
  <li><code>a</code> → first element</li>
  <li><code>b</code> → middle elements (as list)</li>
  <li><code>c</code> → last element</li>
</ul>

<p>
Useful for variable-length data and flexible assignments.
</p>

---

<h2>🔁 Iterating Over Tuples (for & while Loops)</h2>

<p>
Since tuples are ordered collections, they support sequential traversal using
<code>for</code> and <code>while</code> loops. Because tuples are immutable, iteration is always
<b>read-only</b> — no structural modification is possible.
</p>

<h3>▶️ Using the <code>for</code> Loop</h3>

<p>
The <code>for</code> loop is the most natural way to iterate over a tuple. It works directly
with elements and does not require index handling.
</p>

<pre>
t = (10, 20, 30, 40)
for x in t:
    print(x)
</pre>

<p>
To access both index and value, use <code>enumerate()</code>:
</p>

<pre>
for i, x in enumerate(t):
    print(i, x)
</pre>

<p>
Iteration uses the iterator protocol, making tuple traversal fast and memory-efficient.
</p>

<h3>🔄 Using the <code>while</code> Loop</h3>

<p>
The <code>while</code> loop iterates using index positions. This is useful when index-based
logic or pointer-style movement is required.
</p>

<pre>
i = 0
while i < len(t):
    print(t[i])
    i += 1
</pre>

<p>
Since tuples cannot change size, the loop boundary remains stable, eliminating
mutation-related bugs common with lists.
</p>

<h3>⚠️ Immutability During Iteration</h3>

<p>
Tuple elements cannot be reassigned during iteration:
</p>

<pre>
for x in t:
    x = x * 2   # does NOT modify the tuple
</pre>

<p>
This only rebinds the local variable <code>x</code>. The original tuple remains unchanged.
To transform values, a new tuple must be created.
</p>
---

<h2>⚠️ Common Pitfalls</h2>

<ul>
  <li>Forgetting the comma in single-element tuples: <code>(5,)</code></li>
  <li>Expecting tuple methods like list methods</li>
  <li>Trying to modify tuple elements directly</li>
  <li>Confusing immutability with deep immutability (mutable items inside tuple can still change)</li>
</ul>

---

<h2>🎯 When to Use Tuples</h2>

<ul>
  <li>Returning multiple values from functions</li>
  <li>Fixed configuration data</li>
  <li>Dictionary keys</li>
  <li>Data records that should not change</li>
  <li>Performance-critical read-only collections</li>
</ul>

---

<h2>📂 Files in This Folder</h2>

<p>
This folder contains examples demonstrating:
</p>

<ul>
  <li>Tuple creation and indexing</li>
  <li>Packing and unpacking patterns</li>
  <li>Extended unpacking</li>
  <li>Immutability behavior</li>
  <li>Real-world usage scenarios</li>
</ul>

<hr/>

<p align="center">
  <i>Tuples are promises. Once made, they are kept.</i>
</p>
