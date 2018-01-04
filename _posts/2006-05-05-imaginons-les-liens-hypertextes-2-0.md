---
layout: post
title: 'Imaginons les liens hypertextes 2.0'
date: '2006-05-05 12:00:36'
author: j0k
tags: '[]'
excerpt: "Avant, dans le web 1.0, tout les webmasters voulaient savoir qui visitait leur site, qui revenait régulièrement, etc ... C'est ainsi que sont nés les outils de statistiques basés sur les logs des serveurs ou sur un marqueur placé sur chaque page.     \nLa méthode du web 2.0 pour tracker les visiteurs attribue un id à chaque page. Cet id est référencé dans la base      …"
---

Avant, dans le web 1.0, tout les webmasters voulaient savoir qui visitait leur site, qui revenait régulièrement, etc ... C'est ainsi que sont nés les outils de statistiques basés sur les logs des serveurs ou sur un marqueur placé sur chaque page.
La méthode du web 2.0 pour tracker les visiteurs attribue un id à chaque page. Cet id est référencé dans la base de donne avec l'url de la page correspondante. Tous les liens hypertextes deviennent donc :   **HTML**   ``<div class="html4strict"><span class="sc2"><a target="_blank"&nbsp; href="http://december.com/html/4/element/a.html"><span class="kw2">&lt;a</a> <span class="kw3">href=<span class="st0">"Javascript: followLink(124);"<span class="kw2">&gt;</a>View Products<span class="sc2"><span class="kw2">&lt;/a&gt;</div>``   Quand l'utilisateur clique sur le lien, la fonction followLink() exécute le code suivant :

* un div transparent se place sur toute la page avec une sorte de fond grisé et ...
* un message &quot;Veuillez patienter&quot; avec une image de chargement est placé en haut de ce div, et ...
* l'objet XmlHttpRequest est appelé et va ...
* ouvrir une connexion à la base de données pour ...
* archivé le requête et ...
* récupéré l'url correspondant à l'id envoyé puis ...
* retourné tout ça au client qui ...
* renseigne le window.location avec l'url prise dans la base ce qui fait que ...
* l'utilisateur est dirigé vers la page qu'il a demandé.

Ok la [méthode](http://thedailywtf.com/forums/70666/ShowPost.aspx) n'est pas super, mais c'est marrant de voir ce que l'on peut penser du 2.0 !