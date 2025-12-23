<h1 align="center">🐍 Python Lists</h1>

<p align="center">
  <b>Mutable, ordered collections used to store and manipulate grouped data in Python</b>
</p>

<hr/>

<h2>📘 Overview</h2>

<li>
A <b>list</b> is an ordered, mutable collection of elements in Python, created using square
brackets (<code>[ ]</code>) or the <code>list()</code> constructor.
</li>

<li>
Lists are a core data structure and are extensively used in data processing, feature engineering,
algorithm design, and general-purpose programming.
</li>

<li>
Unlike strings and tuples, lists are <b>mutable</b>. Their contents can be modified in place
without creating a new object in memory.
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
    <td>Square brackets <code>[ ]</code> or <code>list()</code></td>
  </tr>
  <tr>
    <td>Mutability</td>
    <td><b>Mutable</b> (elements can be added, removed, or replaced)</td>
  </tr>
  <tr>
    <td>Order</td>
    <td>Insertion order is preserved</td>
  </tr>
  <tr>
    <td>Indexing</td>
    <td>Supports zero-based and reverse indexing (negative)</td>
  </tr>
  <tr>
    <td>Slicing</td>
    <td>Supported (returns a <b>new list</b>)</td>
  </tr>
  <tr>
    <td>Duplicates</td>
    <td>Allowed</td>
  </tr>
  <tr>
    <td>Heterogeneous</td>
    <td>Can store mixed data types</td>
  </tr>
</table>

---

<h2>🧱 Mutability Explained</h2>

<p>Lists <b>do</b> support:</p>

<ul>
  <li>Adding elements</li>
  <li>Removing elements</li>
  <li>Replacing elements at existing indexes</li>
</ul>

<p>
Operations such as <code>append()</code>, <code>insert()</code>, <code>remove()</code>,
and index assignment modify the <b>same list object in memory</b>.
</p>

<p>
This makes lists powerful — and dangerous — when references are shared.
</p>

---

<h2>🔍 Accessing Elements</h2>

<ul>
  <li>Index-based access</li>
  <li>Negative indexing</li>
  <li>Slicing to extract sublists</li>
  <li>Step-based slicing (skipping elements)</li>
</ul>

<p>
<b>Important:</b> Slicing always returns a <b>new list</b>, while index assignment modifies
the original list.
</p>

---

<h2>🧠 List Operations by Memory Behavior</h2>

<h3>➕ Adding Elements (Expands Existing Memory)</h3>

<pre>
append()
extend()
insert()
</pre>

<p>
These operations modify the list <b>in place</b> and increase its size.
They return <code>None</code>.
</p>

---

<h3>➖ Removing Elements (Shrinks Existing Memory)</h3>

<pre>
remove()
pop()
del
</pre>

<p>
These operations remove elements from the same list object.
<code>pop()</code> returns the removed element.
</p>

---

<h3>🧹 Clearing Elements (Contents Removed, Object Retained)</h3>

<pre>
clear()
</pre>

<p>
Removes all elements from the list while preserving the list object and its references.
</p>

---

<h3>📄 Copying Lists (New Memory Allocation)</h3>

<pre>
copy()
list()
[:]
</pre>

<p>
Creates a <b>new list object</b>. This is a <b>shallow copy</b>;
nested objects are still shared.
</p>

---

<h3>🔁 Reordering Elements (Memory Stable, Order Changes)</h3>

<pre>
sort()
reverse()
sorted()
</pre>

<p>
<code>sort()</code> and <code>reverse()</code> mutate the list in place.
<code>sorted()</code> returns a new list.
</p>

---

<h3>🚫 Non-Mutating Operations (Read-Only)</h3>

<pre>
len()
count()
index()
in / not in
</pre>

<p>
These operations inspect the list without modifying it.
</p>

---

<h2>⚠️ Common Pitfalls</h2>

<ul>
  <li>Expecting list methods to return the modified list</li>
  <li>Modifying a list while iterating over it</li>
  <li>Confusing shallow copies with independent copies</li>
  <li>Unintentionally sharing references between variables</li>
  <li>Using lists where sets or tuples are more appropriate</li>
</ul>

---

<h2>🎯 When to Use Lists</h2>

<ul>
  <li>When order matters</li>
  <li>When duplicate values are required</li>
  <li>When frequent insertions or deletions are expected</li>
  <li>When in-place modification is desired</li>
  <li>When flexibility and readability matter more than raw performance</li>
</ul>

---

<h2>📂 Files in This Folder</h2>

<p>
This folder contains Python files and notebooks demonstrating:
</p>

<ul>
  <li>List creation and indexing</li>
  <li>Slicing and step-based access</li>
  <li>Mutation and in-place operations</li>
  <li>Copying vs shared references</li>
  <li>Common list-based problem patterns</li>
</ul>

<hr/>

<p align="center">
  <i>Power with responsibility. Mutability with awareness.</i>
</p>
