# comparison of wiki software

* dokuwiki is stable, can be customized with plugins. but the syntax is weird and i'd have to learn that. + for no database
* bookstack looks somewhat pretty but too much like material ui (i dont like material ui, especially on desktop/web). the hierarchy seems arbitrary and i dont like it.
* wiki.js is material ui garbage
* mediawiki is too much for my needs
* moinmoin i dont like the look
* tiddlywiki manages to looks worse than material ui and has a weird name? like huh??
* xwiki is java. case closed

what i need:
* no database, file based
* markdown based (idc about wysiwyg editor)
* good for a single user
* editable on the web, maybe
* pages can interlink easily
* has version history

observations: most wiki software is either so old that it's written in php or 'new' (and plagued by material ui) that it's nodejs :/

with php > nodejs.

also i refuse to self host nodejs software on my server.

update: this is now on netlify with hugo, despite me complaining about hugo in a blog post from some time ago. it's just too easy: forked a theme, ripped out all the parts i didn't need and voilà. a custom-built system with search and all would've cost too much time.
