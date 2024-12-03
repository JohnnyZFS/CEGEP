# CEGEP
Base de données cegep
1.Executer le fichier tables dans le dossier creation de base de donnees ou se trouve le shema relation
2.Executer les fichiers (Cours,Etudiant,Professeur) dans le dossiers donnees de Creation base donnees
3.Executer le fichier Inscription_Enseignement dans le meme dossier
4.Executer le fichier chiffrement pour la table Professeurs
5.Executer le fichier Traitements_auto qui contient les traitements automatises
6.Executer le fichier utilisateurs dans le dossier gestion des acces ou se trouve le tableau de autorisations
7.Executer les fichiers des autorisations etudiant et professeur dans le dossier Autorisations

Plan de sauvegarde dans le dossier Sauvegarde

Fichier REQUETES avec les 5 besoins

Informations connection

-- Créer l'utilisateur pour l'administration
CREATE LOGIN admin_user WITH PASSWORD = 'Admin2024!'; 
CREATE USER admin_user FOR LOGIN admin_user;  

-- Créer l'utilisateur pour l'étudiant
CREATE LOGIN etudiant_user WITH PASSWORD = 'Etudiant2024!';  -- Créer un login avec un mot de passe sécurisé
CREATE USER etudiant_user FOR LOGIN etudiant_user;  -- Créer un utilisateur dans la base de données

-- Créer l'utilisateur pour le professeur
CREATE LOGIN professeur_user WITH PASSWORD = 'Professeur2024!';  -- Créer un login avec un mot de passe sécurisé
CREATE USER professeur_user FOR LOGIN professeur_user;  -- Créer un utilisateur dans la base de données
