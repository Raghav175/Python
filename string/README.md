<h1 align="center">🐍 Python Strings</h1>

<p align="center">
  <b>Immutable, ordered sequences of characters used for text processing in Python</b>
</p>

<hr/>

<h2>📘 Overview</h2>

<li>
A <b>string</b> is an ordered, immutable sequence of characters in Python, enclosed within
single (<code>' '</code>) or double (<code>" "</code>) quotes.
</li>

<li>
Strings are a core data type and are extensively used in text processing, data cleaning, Natural Language Processing(NLP)
Feature engineering, and input/output operations.
</li>

<li>
Once created, a string cannot be modified in place. Any operation that appears to change a
string actually creates a <b>new string object in memory</b>.
</li>

---

<h2>🧬 Key Characteristics</h2>

<table>
  <tr>
    <th align="left">Property</th>
    <th align="left">Description</th>
  </tr>
  <tr>
    <td>Order</td>
    <td>Characters maintain insertion order</td>
  </tr>
  <tr>
    <td>Mutability</td>
    <td><b>Immutable</b> (existing memory cannot be changed)</td>
  </tr>
  <tr>
    <td>Indexing</td>
    <td>Supports zero-based and negative indexing</td>
  </tr>
  <tr>
    <td>Slicing</td>
    <td>Supported (returns a new string)</td>
  </tr>
  <tr>
    <td>Duplicates</td>
    <td>Allowed</td>
  </tr>
  <tr>
    <td>Creation</td>
    <td>Single or double quotes</td>
  </tr>
</table>

---

<h2>🔍 Accessing Characters</h2>

<ul>
  <li>Index-based access</li>
  <li>Negative indexing</li>
  <li>Slicing to extract substrings</li>
  <li>Step-based slicing (skipping characters)</li>
</ul>

<p>
<b>Important:</b> Slicing always returns a new string and never modifies the original.
</p>

---

<h2>🧱 Immutability Explained</h2>

<p>Strings do <b>not</b> support:</p>

<ul>
  <li>Adding characters to existing memory</li>
  <li>Deleting characters from existing memory</li>
</ul>

<p>
Operations such as concatenation or replacement create a <b>new string object</b>.
This design improves memory safety and enables internal optimizations in Python.
</p>

---

<h2>🛠 Common String Operations</h2>

<pre>
len()
capitalize()
title()
lower()
upper()
copy()
replace()
</pre>

<p>
All string methods return a <b>new string</b> or a derived value.
</p>

---

<h2>✅ Membership & Validation</h2>

<pre>
in
startswith()
endswith()
isnumeric()
isalpha()
isalnum()
islower()
isupper()
</pre>

<p>
These methods always return a <code>True</code> or <code>False</code> value.
</p>

---

<h2>🔢 ASCII & Character Utilities</h2>

<pre>
ord()  → Character to ASCII
chr()  → ASCII to Character
</pre>

<p>
Used in encoding, decoding, and low-level string manipulation.
</p>

---

<h2>⚠️ Common Pitfalls</h2>

<ul>
  <li>Assuming strings can be modified in place</li>
  <li>Expecting <code>.replace()</code> to change the original string</li>
  <li>Forgetting slicing creates a new object</li>
  <li>Overusing concatenation inside loops</li>
  <li>Confusing string methods with list methods</li>
</ul>

---

<h2>🎯 When to Use Strings</h2>

<ul>
  <li>Text processing and validation</li>
  <li>User input and output handling</li>
  <li>Data cleaning and normalization</li>
  <li>Encoding categorical information</li>
  <li>Log and message processing</li>
</ul>

---

<h2>📂 Files in This Folder</h2>

<p>
This folder contains Python files and notebooks demonstrating:
</p>

<ul>
  <li>String creation and indexing</li>
  <li>Slicing and skipping patterns</li>
  <li>Built-in string methods</li>
  <li>Membership and validation checks</li>
  <li>Practical manipulation examples</li>
</ul>

<hr/>

<p align="center">
  <i>Clarity over cleverness. Immutability over surprises.</i>
</p>

