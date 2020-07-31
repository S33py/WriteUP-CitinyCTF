# Wu-CitinyCTF
Write-up du Citiny-CTF section cryptanalyse.
## Début
Salut à tous, aujourd'hui je vous présente mon WU du CitinyCTF présenté dans un prog CLI, c'est un CTF de cryptanalyse et un peu de RE au début. Le concept était assez drôle, il m'a fallu beaucoup de temps pour cerner la logique de certains challenges, dont le dernier qui était vraiment casse tête. Au final j'ai réussi donc plus de bien que de mal. 
## Unpacking UPX
La première étape consistait à bypass le GetDlgItemText() importé par user32.dll où il nous demande d'insérer un mot de passe pour accéder au CTF. </br><br/>
<img src="https://media.discordapp.net/attachments/736536361258975253/738879854207959133/unknown.png"/><br/><br/>
J'ai donc essayé de voir en quoi le prog était packé, pour ce faire je l'ai d'abord désasemblé 
