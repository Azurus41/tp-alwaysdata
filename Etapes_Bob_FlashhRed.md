# TP1 – Partie de Bob (Ewen Guillon, compte GitHub FlashhRed)

À faire sur le PC d'Ewen, après avoir accepté l'invitation reçue par e-mail
(ou sur https://github.com/Azurus41/tp-alwaysdata/invitations).

```bash
git config --global user.name "FlashhRed"
git config --global user.email "<e-mail du compte FlashhRed>"

git clone https://github.com/Azurus41/tp-alwaysdata.git
cd tp-alwaysdata
git switch bob
```

Modifier `script.js`, par exemple ajouter à la fin :

```js
console.log("Modification de Bob (FlashhRed) depuis son PC");
```

```bash
git add script.js
git commit -m "Bob : ajout d'un log JS depuis le PC de Bob"
git push
```

Puis fusion dans master (par Ewen ou par Azur) :

```bash
git switch master
git pull
git merge bob -m "Merge branche bob dans master"
git push
git log --oneline --graph --all
```

Captures à faire pour le compte rendu : le `git clone`, le `git push` de Bob,
et le graphe final (`git log --graph` ou Insights → Network sur GitHub),
où l'on voit les commits des deux auteurs.
