<h1 align="center">🐍 Python Dictionaries</h1>

<p align="center">
  <b>Mutable, unordered collections of key–value pairs for fast lookups</b>
</p>

<hr/>

<h2>📘 Overview</h2>

<li>
A <b>dictionary</b> (<code>dict</code>) is a built-in Python data structure used to store data
in <b>key–value pairs</b>.
</li>

<li>
Dictionaries are enclosed in curly braces <code>{ }</code>, where each key is mapped to a value
using a colon (<code>:</code>) and pairs are separated by commas (<code>,</code>).
</li>

<li>
They are optimized for <b>fast retrieval, insertion, and updates</b> based on keys.
</li>

<li>
<b>Keys must be unique and hashable.</b> Duplicate keys are <b>not allowed</b>.
If a key is repeated, the last assigned value silently overwrites the previous one.
</li>

---

<h2>🧬 Key Characteristics</h2>

<table>
  <tr>
    <th align="left">Property</th>
    <th align="left">Description</th>
  </tr>
  <tr>
    <td>Collection Type</td>
    <td>Key–Value pairs</td>
  </tr>
  <tr>
    <td>Mutability</td>
    <td><b>Mutable</b> (can be modified in place)</td>
  </tr>
  <tr>
    <td>Order</td>
    <td>Unordered (insertion order preserved internally since Python 3.7, but not index-based)</td>
  </tr>
  <tr>
    <td>Indexing</td>
    <td>Key-based access only (no positional indexing)</td>
  </tr>
  <tr>
    <td>Duplicate Keys</td>
    <td><b>Not Allowed</b></td>
  </tr>
  <tr>
    <td>Duplicate Values</td>
    <td>Allowed</td>
  </tr>
</table>

---

<h2>🧱 Mutability Explained</h2>

<p>Dictionaries <b>can be modified in place</b>, meaning:</p>

<ul>
  <li>New key–value pairs can be added</li>
  <li>Existing values can be updated</li>
  <li>Keys can be removed</li>
</ul>

<p>
Unlike strings and tuples, dictionary operations typically modify the same object
instead of creating a new one.
</p>

---

<h2>🔍 Accessing Data</h2>

<ul>
  <li>Access values using keys</li>
  <li>Safe access using <code>.get()</code></li>
  <li>Iterate over keys, values, or both</li>
</ul>

<p>
<b>Important:</b> Accessing a missing key directly raises a <code>KeyError</code>.
Use <code>.get()</code> when safety matters.
</p>

---

<h2>🛠 Common Dictionary Methods</h2>

<pre>
.get()
.update()
.pop()
.popitem()
</pre>

<p>
These methods are used for safe access, updates, and controlled removal of data.
</p>

---

<h2>🔄 Dictionary Views</h2>

<pre>
.keys()
.values()
.items()
</pre>

<p>
These return <b>dynamic view objects</b> that reflect changes made to the dictionary
in real time.
</p>

---

<h2>🧹 Utility Methods</h2>

<pre>
.copy()
.clear()
</pre>

<ul>
  <li><code>.copy()</code> creates a shallow copy</li>
  <li><code>.clear()</code> removes all key–value pairs</li>
</ul>

---

<h2>🚫 Rules & Constraints</h2>

<ul>
  <li>Keys must be immutable (e.g., int, str, tuple)</li>
  <li>Lists, sets, and dictionaries cannot be keys</li>
  <li>No duplicate keys allowed</li>
  <li>Duplicate key–value pairs are impossible by definition</li>
</ul>

<p>
If the same key appears multiple times, the <b>last assignment wins</b>.
</p>

---

<h2>⚠️ Common Pitfalls</h2>

<ul>
  <li>Expecting index-based access like lists</li>
  <li>Forgetting that duplicate keys overwrite silently</li>
  <li>Using mutable objects as keys</li>
  <li>Assuming dictionaries are sorted</li>
  <li>Modifying a dictionary while iterating over it</li>
</ul>

---

<h2>🎯 When to Use Dictionaries</h2>

<ul>
  <li>Fast lookups by identifier</li>
  <li>Configuration and settings storage</li>
  <li>JSON-like structured data</li>
  <li>Counting and frequency analysis</li>
  <li>Mapping relationships between entities</li>
</ul>

---

<h2>📂 Files in This Folder</h2>

<p>
This folder contains examples covering:
</p>

<ul>
  <li>Dictionary creation and updates</li>
  <li>Safe access patterns</li>
  <li>Iteration over keys and values</li>
  <li>Real-world mapping use cases</li>
  <li>Performance-friendly lookup patterns</li>
</ul>

<hr/>

<p align="center">
  <i>Keys define meaning. Values carry state.</i>
</p>
