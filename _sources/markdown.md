# Definisi Sistem Persamaan Linier
Pada subbab ini akan dibahas definisi sistem persamaan linear beserta contoh sistem persamaan linear. Sebelum dibahas tentang sistem persamaan linear, lebih dulu akan diberikan definisi persamaan linear.

Yang dimaksud dengan persamaan linear dalam n variabel (unknown, anu) x_{1}, x_{2} ,...,x n adalah persamaan dengan bentuk umum

a_{1}*x_{1} + a_{2}*x_{2} +...+a n x n =b

dengan a_{1}, a_{2} ,...,a n , b menyatakan bilangan-bilangan real dan tidak semua a, i = 1, 2 ,...,n adalah nol. Untuk semua i = 1, 2 ,...,n, bilangan a_{i} disebut sebagai koefisien variabel x_{i} dan b disebut sebagai suku konstan.
## What is MyST?

MyST stands for "Markedly Structured Text". It
is a slight variation on a flavor of markdown called "CommonMark" markdown,
with small syntax extensions to allow you to write **roles** and **directives**
in the Sphinx ecosystem.

For more about MyST, see [the MyST Markdown Overview](https://jupyterbook.org/content/myst.html).

## Sample Roles and Directives

Roles and directives are two of the most powerful tools in Jupyter Book. They
are like functions, but written in a markup language. They both
serve a similar purpose, but **roles are written in one line**, whereas
**directives span many lines**. They both accept different kinds of inputs,
and what they do with those inputs depends on the specific role or directive
that is being called.

Here is a "note" directive:

```{note}
Here is a note
```

It will be rendered in a special box when you build your book.

Here is an inline directive to refer to a document: {doc}`markdown-notebooks`.


## Citations

You can also cite references that are stored in a `bibtex` file. For example,
the following syntax: `` {cite}`holdgraf_evidence_2014` `` will render like
this: {cite}`holdgraf_evidence_2014`.

Moreover, you can insert a bibliography into your page with this syntax:
The `{bibliography}` directive must be used for all the `{cite}` roles to
render properly.
For example, if the references for your book are stored in `references.bib`,
then the bibliography is inserted with:

```{bibliography}
```

## Learn more

This is just a simple starter to get you started.
You can learn a lot more at [jupyterbook.org](https://jupyterbook.org).
