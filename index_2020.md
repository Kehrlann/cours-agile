<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no"
    />

    <title>Méthodes de développement</title>

    <link rel="stylesheet" href="css/reset.css" />
    <link rel="stylesheet" href="css/reveal.css" />
    <link rel="stylesheet" href="css/theme/white.css" />

    <!-- Theme used for syntax highlighting of code -->
    <link rel="stylesheet" href="lib/css/monokai.css" />

    <!-- Printing and PDF exports -->
    <script>
      var link = document.createElement("link");
      link.rel = "stylesheet";
      link.type = "text/css";
      link.href = window.location.search.match(/print-pdf/gi)
        ? "css/print/pdf.css"
        : "css/print/paper.css";
      document.getElementsByTagName("head")[0].appendChild(link);
    </script>
    <style type="text/css">
      .reveal section img {
        border: none;
        background: none;
        box-shadow: none;
      }

      .reveal .centering {
        width: 100%;
        text-align: center;
      }

      .reveal pre code {
        padding: 24px;
        max-height: none;
      }

      .reveal h2 {
        margin-bottom: 1em;
      }

      #profile-pic {
        height: 300px;
        border-radius: 50%;
      }
    </style>
  </head>
  <body>
    <div class="reveal">
      <div class="slides">
        <section data-markdown>
          <textarea data-template>
            # Méthodes agiles

            <br>

            ## Process et méthodes de développement logiciel

            <br>
            <br>

            #### Mines Paristech
            #### 09 / 03 / 2020
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Daniel Garnier-Moiroux

            <img src="images/profile_picture.jpeg" id="profile-pic">
            <br>

            Software Engineer @ Pivotal Labs

            [@Kehrlann](https://twitter.com/Kehrlann)

            https://github.com/Kehrlann

            daniel@garnier.wf
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Aujourd'hui, du logiciel partout

            <img src="images/issues_de_secours.png" height="600px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Plan

            1. Introduction
            2. Historique des projets logiciels et des méthodos
            3. Philosophie de "l'agilité"
            4. Quelques exemples de Méthodes Agiles™
            5. Exercice pratique
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            # Historique des projets software
          </textarea>
        </section>
        <section data-markdown data-background-image="images/colossus.jpg" data-background-size="contain">
        </section>
        <section data-markdown data-background-image="images/apollo.jpg" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            ## "Software crisis"

            <br>

            > The major cause of the software crisis is that the machines have become several orders of magnitude more powerful! To put it quite bluntly: as long as there were no machines, programming was no problem at all; when we had a few weak computers, programming became a mild problem, and now we have gigantic computers, programming has become an equally gigantic problem.
            >
            > — Edsger Dijkstra, The Humble Programmer (EWD340), Communications of the ACM (1972)
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Quelques statistiques

            A votre avis, combien de projets logiciels sont:
            - Des réussites ?
            - Des échecs complets ?
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Standish Group "Chaos Report"

            <img src="images/stats-standish-1.jpg" height="500px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Quelques statistiques

            - Coût de développement = moitié du coût opération + maintenance
            - 50% des projets sont opérationnels, mais pas "réussis"
            - Projet moyen: +50% de budget
          </textarea>
        </section>
        <section data-markdown data-background-image="images/system-360.jpg" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            ## IBM System/360

            > Ajouter des développeurs à un projet en retard aggrave le retard
            >
            > Fred Brooks, "The Mythical Man-Month", 1975
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            # Historique des méthodologies
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## 1960s "software engineering"

            <img src="images/margaret-hamilton.jpg" height="900px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## 1970: "Managing the development of large software systems"

            Article publié par Winston W. Royce, directeur de "Lockheed Software Technology Center"

            <img src="images/winston-w-royce.jpg" height="600px">
          </textarea>
        </section>
        <section data-markdown data-background-image="images/waterfall.png" data-background-size="contain">
        </section>
        <section data-markdown data-background-image="images/cost-of-change.gif" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            > I believe in this concept but the implemention described above is risky and invites failure.
            >
            > Winston W. Royce
          </textarea>
        </section>
        <section data-markdown data-background-image="images/waterfall-complete.png" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Une variation: le cycle en V

            <img src="images/v-model.jpg" height="900px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Scrum (1995)

            - 1986, "The New New product development game", HBR, Takeuchi & Nonaka
            - 1995, Ken Schwaber & Jeff Sutherland présentent "Scrum development process" à [OOPSLA '95](http://jeffsutherland.com/oopsla/oo95wrkf.html)
            - 2001, livre "Agile software development with Scrum", Schwaber & Beedle
            - Idée principale: des développements **itératifs**

            <br>
            <br>

            <img src="images/scrum-book.jpg" height="500px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## eXtreme Programming (XP) Explained, _Embrace Change_ (1999)

            - Kent Beck
            - Idée principale: des **valeurs**, pour organiser une équipe de développement

            <br>
            <br>

            <img src="images/xp-explained.jpg" height="500px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Manifeste Agile (2001)

            - Idées solides sur ce qui fonctionne pour **fabriquer du logiciel qui fonctionne**
            - https://agilemanifesto.org
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Lean Software Development (2003)

            - Mary & Tom Poppendieck
            - Basé sur le "lean manufacturing"
            - Idée importante: autonomie de l'équipe, on doit leur donner **des problèmes à résoudre, pas des solutions**

            <br>
            <br>

            <img src="images/lean-software-development.jpg" height="500px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Toyota Kata (2009)

            - Mike Rother
            - Idées intéressantes autour du **management**

            <br>
            <br>

            <img src="images/toyota-kata.jpg" height="700px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## The Lean Startup (2011)

            - Eric Ries
            - Idée: il faut du lean aussi **dans le développement produit**

            <br>
            <br>

            <img src="images/lean-startup.jpg" height="700px">
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            # Valeurs et principes "agiles"
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## https://agilemanifesto.org
          </textarea>
        </section>
        <section data-markdown data-background-image="images/de-risk-1.png" data-background-size="contain">
        </section>
        <section data-markdown data-background-image="images/de-risk-2.png" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            # ⏰ PAUSE ⏰
          </textarea>
        </section>
        <section data-markdown data-background-image="images/lean-startup.jpg" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            <img src="images/agile-car.png" height="700px">
          </textarea>
        </section>
        <section data-markdown data-background-image="images/discovery-and-framing.png" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            # Méthodes particulières
          </textarea>
        </section>
        <section data-markdown data-background-image="images/scrum-1.jpg" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            <img src="images/stand-up.jpg" height="900px">
          </textarea>
        </section>
        <section data-markdown data-background-image="images/user-story-1.png" data-background-size="contain">
        </section>
        <section data-markdown data-background-image="images/user-story-2.png" data-background-size="contain">
        </section>
        <section data-markdown data-background-image="images/user-story-3.png" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            <img src="images/retro-happy-meh-sad.png" height="740px">
          </textarea>
        </section>
        <section data-markdown data-background-image="images/retro-boat-2.jpg" data-background-size="contain">
        </section>
        <section data-markdown data-background-image="images/kanban.png" data-background-size="contain">
        </section>
        <section data-markdown data-background-image="images/safe.png" data-background-size="contain">
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Des opinions fortes ...

            [Beware SAFe, an unholy incarnatation of darkness](https://medium.com/@seandexter1/beware-safe-the-scaled-agile-framework-for-enterprise-an-unholy-incarnation-of-darkness-bf6819f6943f)
          </textarea>
        </section>
        <section data-markdown>
          <textarea data-template>
            ## Exemples

            > Il s'agirait d'un jeu vidéo de type RPG (Role Playing Game)
            > Entre autre, je compte prévoir:
            >
            > - un système de sauvegarde de l'aventure, cela me ferait utiliser les écritures et lectures de fichiers.
            > - différentes interfaces graphiques, pour la répartition des points gagnés lorsque le personnage monte d'un niveau, ou pour lancer des sorts, car j'aimerais que le joueur puisse dessiner des incantations pour pouvoir les lancer, et que l'algorithme les reconnaisse.
            > - la gestion de différents métiers, de différentes ressources dans le jeu
            > - des combats au tour par tour contre l'ordinateur
          </textarea>
        </section>
      </div>
    </div>

    <script src="js/reveal.js"></script>

    <script>
      // More info about config & dependencies:
      // - https://github.com/hakimel/reveal.js#configuration
      // - https://github.com/hakimel/reveal.js#dependencies
      Reveal.initialize({
        width: 1400,
        height: 1080,
        history: true,
        transition: "none",
        backgroundTransition: "none",
        hash: true,
        dependencies: [
          { src: "plugin/markdown/marked.js" },
          { src: "plugin/markdown/markdown.js" },
          { src: "plugin/highlight/highlight.js" },
          { src: "plugin/notes/notes.js", async: true }
        ]
      });
    </script>
  </body>
</html>
