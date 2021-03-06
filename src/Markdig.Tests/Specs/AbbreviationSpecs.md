# Extensions

This section describes the different extensions supported:

## Abbreviation

Abbreviation can be declared by using the `*[Abbreviation Label]: Abbreviation description`

Abbreviation definition will be removed from the original document. Any Abbreviation label found in literals will be replaced by the abbreviation description:
 
```````````````````````````````` example
*[HTML]: Hypertext Markup Language

Later in a text we are using HTML and it becomes an abbr tag HTML
.
<p>Later in a text we are using <abbr title="Hypertext Markup Language">HTML</abbr> and it becomes an abbr tag <abbr title="Hypertext Markup Language">HTML</abbr></p>
````````````````````````````````

An abbreviation definition can be indented at most 3 spaces
 
```````````````````````````````` example
*[HTML]: Hypertext Markup Language
    *[This]: is not an abbreviation
.
<pre><code>*[This]: is not an abbreviation
</code></pre>
````````````````````````````````

An abbreviation may contain spaces:
 
```````````````````````````````` example
*[SUPER HTML]: Super Hypertext Markup Language

This is a SUPER HTML document    
.
<p>This is a <abbr title="Super Hypertext Markup Language">SUPER HTML</abbr> document</p>
````````````````````````````````

Abbreviation may contain any unicode characters:

```````````````````````````````` example
*[😃 HTML]: Hypertext Markup Language

This is a 😃 HTML document    
.
<p>This is a <abbr title="Hypertext Markup Language">😃 HTML</abbr> document</p>
````````````````````````````````
