<h1 align="center">🐍 Python Sets</h1>

<p align="center">
  <b>Unordered, mutable collections of unique elements optimized for set logic</b>
</p>

<hr/>

<h2>📘 Definition</h2>

<p>
A <b>set</b> is an <b>unordered collection</b> of items in Python that
<b>does not allow duplicate values</b>.
</p>

<p>
Sets are commonly used for enforcing uniqueness, fast membership testing,
and mathematical set operations.
</p>

---

<h2>🧱 Syntax</h2>

<p>
Sets are enclosed in <code>{ }</code> and elements are separated by commas <code>,</code>
</p>

<pre>
my_set = {1, 2, 3, 4}
</pre>

<p>
To create an empty set:
</p>

<pre>
empty_set = set()
</pre>

---

<h2>🧬 Key Properties</h2>

<table>
  <tr>
    <th align="left">Property</th>
    <th align="left">Value</th>
  </tr>
  <tr>
    <td>Mutability</td>
    <td>Mutable</td>
  </tr>
  <tr>
    <td>Order</td>
    <td>Unordered</td>
  </tr>
  <tr>
    <td>Duplicates</td>
    <td>Not Allowed</td>
  </tr>
  <tr>
    <td>Indexing</td>
    <td>Not Supported</td>
  </tr>
</table>

---

<h2>➕ Adding Elements</h2>

<pre>
.add()
.update()
</pre>

<p>
Used to insert new elements into a set.
</p>

---

<h2>➖ Removing Elements</h2>

<pre>
.remove()
.discard()
.pop()
</pre>

<p>
<b>Note:</b><br/>
<code>remove()</code> raises an error if the element does not exist.<br/>
<code>discard()</code> does not raise an error.<br/>
<code>pop()</code> removes and returns an arbitrary element.
</p>

---

<h2>🧰 Utility Methods</h2>

<pre>
.copy()
.clear()
</pre>

<p>
Used for duplicating or resetting sets.
</p>

---

<h2>🧮 Mathematical Set Operations</h2>

<pre>
.union()
.intersection()
.difference()
.symmetric_difference()
</pre>

<p>
Used for combining, comparing, and filtering sets.
</p>

---

<h2>🔁 In-place Set Updates</h2>

<pre>
.update()
.intersection_update()
.difference_update()
.symmetric_difference_update()
</pre>

<p>
These methods modify the original set instead of returning a new one.
</p>

---

<h2>🔍 Set Relationship Checks</h2>

<pre>
.issubset()
.issuperset()
.isdisjoint()
</pre>

<p>
Used to compare relationships between two sets.
</p>

---

<h2>⚠️ Important Notes</h2>

<ul>
  <li>Sets do not maintain insertion order</li>
  <li>Indexing and slicing are not supported</li>
  <li>Elements inside a set must be immutable</li>
  <li><code>pop()</code> does not remove a predictable element</li>
</ul>

---

<h2>🎯 When to Use Sets</h2>

<ul>
  <li>Removing duplicate values</li>
  <li>Fast membership testing</li>
  <li>Comparing datasets</li>
  <li>Filtering elements</li>
  <li>Implementing mathematical set logic</li>
</ul>

<hr/>

<p align="center">
  <i>Uniqueness enforced. Order sacrificed. Logic empowered.</i>
</p>
