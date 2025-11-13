# Git a GitHub tutorial pre začiatočníkov

### Inštalácia

Stiahnem a nainštalujem - [GIT](https://git-scm.com/)

Otestujem inštaláciu
```
git --version
```

Nastavím meno a email
```
git config --global user.name "Meno"
git config --global user.email "Email"
```

---

### Základné príkazy
Vytvorím lokálny repozitár.
```
git init
```  
Stav projektu - čo sa zmenilo.
```
git status
```
Pridám súbor, ktorý chcem mať v novej verzii. 
```
git add index.html 
git add .
```
Vytvorím novú verziu. 🎉 **Vždy pridám popis!**
```
git commit -m ""
```

---

#### Ďalšie príkazy

Zruším pridanie súborov.
```
git restore --staged .
```
Log commitov.
```
git log
git log --graph
git log --graph --abbrev-commit --pretty=oneline
```

Zmeny, ktore som aktuálne urobil oproti GIT-u.
```
git diff
```

Zmena medzi verziami súborov. 
```
git checkout -- index.html  : ak chces vratit zmenu suboru na tu, co bola pri commite
git checkout (commit hash)  : skocim do starej verzie
git checkout master         : vratim sa na koniec
```

---

#### GIT vo VS Code

---

#### GitHub 
Naklonovanie existujúceho repozitára zo servera.
```
git clone https://github.com/...
```

Vytvorit odkaz na konkrétny repozitár na serveri.
```
git remote add origin https://...
```

Nahrať zmeny lokálneho repozitára na server.
```
git push -u origin master
git push origin master
```

Stiahnuť najnovšie súbory zo servera.
```
git pull orgin master 
```

Skontrolovať stav repozitára na serveri oproti môjmu lokálnemu.
```
git remote update
```
---

#### Konflikt  

---

#### Vetvy 

Zobraziť všetky vetvy.
```
git branch
```

Vytvoriť novú vetvu.
```
git branch nova_branch
```

Prepnúť sa do vetvy.
```
git checkout nova_branch
```

Prepnúť sa do novej vetvy dalsia_branch.
```
git checkout -b dalsia_branch
```

Zlúčiť zmeny medzi vetvami. Zlúči zmeny z dalsia_branch do vetvy, v ktorej sa nachádzam. 
```
git merge dalsia_branch
```

[Merge vs Rebase](https://www.atlassian.com/git/tutorials/merging-vs-rebasing)

---

#### Gitignore

[.gitignore generator](https://www.toptal.com/developers/gitignore)
