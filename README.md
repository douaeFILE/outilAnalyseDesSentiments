💬 Projet d’Analyse des Sentiments sur le Conflit Palestine-Israël
Par Douae Laayouni et Oumaima Ihrissane

Ce projet vise à analyser les sentiments exprimés autour du conflit Palestine-Israël, en utilisant des techniques de traitement automatique du langage (NLP) et des outils de visualisation web.

🧠 Objectif
Sensibiliser et donner de la visibilité aux opinions concernant la Palestine à travers l’analyse des tweets et commentaires liés aux trois thèmes : Hamas, Israël, et Conflit.

🔧 Étapes principales
Choix du sujet :
Après avoir analysé plusieurs projets existants, nous avons choisi un thème original centré sur l’actualité du conflit en Palestine.

Collecte de données :
N’ayant pas pu exploiter l’API de Twitter (limitations de compte), nous avons téléchargé des datasets depuis Kaggle (hamas1_export.csv, israel1_export.csv, conflit1_export.csv).

Création de la base de données :
Base MySQL sentiment_analyse, avec tables créées via un script Python. Données nettoyées puis insérées dans les tables hamas1, israel1, conflit1.

Analyse des sentiments :

Traitement des textes avec VADER (outil NLP).

Résultats insérés dans hamas2, israel2, conflit2 avec le champ sentiment.

Interface utilisateur avec Tkinter :

Écran de login/signup (utilisateurs enregistrés dans la table users).

Choix d’un thème (Hamas, Israël, Conflit).

Lancement d’une page PHP via webbrowser (connexion Tkinter → PHP).

Visualisation des résultats (PHP + Chart.js) :

Graphiques (courbes, barres, camemberts, nuages de mots).

Fichier sentiment_results.php.

Historique des utilisateurs :

Table user_logs enregistrant l’email, le thème choisi et la date.

Page admin_dashboard.php pour consulter/supprimer son propre historique.

Commentaires interactifs :

Formulaire comment_form.php permettant à l’utilisateur d’ajouter son avis.

Analyse via analyse_sentiment_comment.py.

Stockage dans user_comments (email, texte, sentiment, thème, date).

Visualisation dynamique des commentaires avec visualiser_commentaires.php.

Exportation :
Possibilité de télécharger les commentaires en format Excel ou PDF pour un usage futur.

📁 Technologies utilisées
Backend : Python (VADER, Pandas, MySQL Connector)

Frontend : PHP, HTML/CSS, Chart.js, Bootstrap

Base de données : MySQL (phpMyAdmin)

Interface locale : Tkinter (Python)
