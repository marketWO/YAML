# YAML
about YAML front matter
jak vypadá a co je to YAML front matter?

  Any file that contains a YAML front matter block will be processed by Jekyll as a special file. The front matter must be the first
  thing in the file and must take the form of valid YAML set between triple-dashed lines. Here is a basic examples:

---
layout: post
title: Blogging Like a Hacker
---

---
title: Using YAML front matter
date: 2016-03-15T02:49:00+00:00
excerpt: "YAML variables can be referenced via liquid tags to add content to template files."
layout: codelog
permalink: /using-yaml-front-matter/
topic: Jekyll
---

---
name: Derek Worthen
age: young
contact:
 email: email@domain.com
 address: some location
pets:
 - cat
 - dog
 - bat
match: !!js/regexp /pattern/gim
run: !!js/function function() { }
---

Between these triple-dashed lines, you can set predefined variables (see below for a reference) or even create custom ones of your own. 
These variables will then be available to you to access using Liquid tags both further down in the file and also in any layouts or includes
that the page or post in question relies on.
__________________________________________________________________________________________________________________________________________
Každý soubor, který obsahuje blok YAML front matter, bude Jekyll zpracovávat jako speciální soubor.
Front matter musí být první věcí v souboru a musí mít podobu platné hodnoty YAML, která je nastavená mezi třemi přerušovanými čárami. 
Příklady:
---
layout: post
title: Blogging Like a Hacker
---

---
title: Using YAML front matter
date: 2016-03-15T02:49:00+00:00
excerpt: "YAML variables can be referenced via liquid tags to add content to template files."
layout: codelog
permalink: /using-yaml-front-matter/
topic: Jekyll
---

---
name: Derek Worthen
age: young
contact:
 email: email@domain.com
 address: some location
pets:
 - cat
 - dog
 - bat
match: !!js/regexp /pattern/gim
run: !!js/function function() { }
---

Mezi těmito třemi přerušovanými čarami můžeme nastavit předdefinované proměnné nebo dokonce vytvořit vlastní. 
Tyto proměnné budou k dispozici pro přístup ke značkám Liquid, a to jak dále v souboru, tak i v jakémkoli rozvržení, nebo zahrnují, 
že daná stránka nebo příspěvek jsou spolehlivé.


Zdroje/Resources
https://protesilaos.com/codelog/using-yaml-front-matter/
https://jekyllrb.com/docs/frontmatter/
https://www.npmjs.com/package/yaml-front-matter
