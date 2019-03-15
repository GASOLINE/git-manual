# git-manual
Voor snelle referentie

# Korte handleiding als naslag
Uitleg Videos:
* https://youtu.be/HfTXHrWMGVY (Setting up git op PC)
* https://youtu.be/IHaTbJPdB-s (Werking Git)

# We moeten dus eerst git op PC opgezet hebben
Opzetten connectie met Github.
* $ git config --global user.name "je naam"
* $ git config --global user.email "je_github@email.ext"

Optional (Voor VScode voor messages)
* $ git config --global core.editor "code --wait"

#  Toevoegen SSH access
Toevoegen SSH access zodat je niet telkens password moet invoeren
* $ ssh-keygen -t rsa -b 4096 -C "je_github@email.ext"

Kopiëren SSH publiek key
* $ xclip -sel clip < ~/.ssh/id_rsa.pub
Die gekopieerde key nu toevoegen aan Github op de Github website onder settings.


# PROJECT opzetten
    
Maak project op Git (leeg) alleen met readme file.

Clone met SSH naar folder op PC.
* $ git clone git@github.com:GASOLINE/git-manual
    
Add new files
* $ git add filname.ext
* $ git add . (=alles)

Opmerkingen erbij zetten
* $ git commit -m “Opmerkingen hier zetten”
    
Zoeken verschillen
* $ git diff
    
Aanpassingen terugzetten naar Github
* $ git push 