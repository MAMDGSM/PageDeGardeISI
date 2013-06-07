Description
----
  "PageDeGardeISI" est un paquage qui permet de générer la page de garde de l'ISI, 
  l'Institut Supérieur d'Informatique de l'Université Tunis El Manar, Ariana, Tunisie.

  La mise en page a été adapté en LaTeX par :
  M. Sabri BAHRINI, M. Moez MAÂMER, M. Med Ali Mortadha DAHMANI, ISI 2013.

Installation
----
1. Créer et Sauvegarder un fichier .tex (vide), encodage UTF-8.
2. Copier/coller le fichier "PageDeGardeISI.sty" dans le même dossier que le .tex (fichier crée précedemment).
3. Ajouter `\usepackage{PageDeGardeISI}` dans le Préambule, à coté des autres `\usepackage`.

Utilisation/Exemple
----
```
\documentclass[a4paper,11pt]{report}
\usepackage{PageDeGardeISI} 

% Diplôme, tel que Licence Appliquée, Ingéniorat Nationale en Informatique
\diplome{Licence Appliquée}

% Option suivis, tel que Systèmes Informatiques et Logiciels, Systèmes Embarqués
\option{Systèmes Informatiques et Logiciels}

% Prénom suivis du nom (si Monôme \prenomNomDe{}{}, si non \prenomNomDe{Foulen}{Ben Foulen})
\prenomNomUn{Foulen}{Ben Foulen}
\prenomNomDe{Foulen}{Ben Foulen}
%\prenomNomDe{}{}

% Sujet/Nom du projet
\sujet{Création et Intégration d'un Système}

% Logo de l'organisme d'accueil (nom de fichier image)
\organismeAccueil{LogoISI.png}

% Nom de l'encadrant de l'entreprise (si le sujet à l'ISI \encadrantEte{}{}, si non \encadrantEte{Foulen}{Ben Foulen})
\encadrantEte{Foulen}{Ben Foulen}
%\encadrantEte{}{}

% Nom de l'encadrant de l'ISI
\encadrantISI{Foulen}{Ben Foulen}

% Année universitaire, de forme AAAA-AAAA
\anneeUniversitaire{2012-2013}

\begin{document}
\makepageDeGarde
\end{document}
```
