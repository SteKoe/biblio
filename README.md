## biblio
biblio is a central bibtex repository which allows you to select bibliography from a central managed repository.
This allows you to reuse existing bibtex definitions without searching for them on your own.

BIBLIO is hostet on GitHub but can as well be installed on premise and be used in your company / university as well.

# Available command line argumens
| Command                          | Description
| --------------------------------	| ----
| ```biblio```                             | Run biblio for your LaTeX Project.
| ```bliblio update```                     | Updates your lokal repository to the latest versions from remote repository.
| ```bliblio config set <key> <value>```   | Set a new value for the given key in your lokal biblio config. Existing values will be overwritten.
| ```bliblio  config get <key>```           | Get the current value of configuration by <key>.

# Standard configuration keys
| Key                          | Description
| ---------------------------- | ----
| remote.repository            | https://github.com/SteKoe/biblio/repo
| local.repository             | ~/.biblio

# Standard repository structure

```/<TYPE>/<AUTHOR>/<YEAR>/<KEY>.bib``` <br>
e.g. ```/book/crumlish/2009/crumlish.2009.bib``` <br>
e.g. ```/book/crumlish/2009/crumlish.2009.[a-z].bib``` <br>

# Usage
When you specify a bib entry without the corresponding body, the information will be pulled from the central repository and added to your lokal repository. If you want to add a source which is not part of the central repository, you might do a pull request and add the missing source, or define a body as usual.

```code
@book{Crumlish.2009.a}
asd
sdfsdf 
dsf
```