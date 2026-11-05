# Backlog de GestiTâches

Ces histoires décrivent les premiers besoins à couvrir. Elles serviront de point de départ aux issues GitHub; les détails pourront être ajustés avec l'équipe avant le développement.

## Sprint 1 — Préparer le projet et les bases

### US-01 — Créer une tâche

**Histoire.** En tant que personne qui utilise GestiTâches, je veux ajouter une tâche avec un titre et une description, afin de garder une trace de ce que j'ai à faire.

**Critères d'acceptation**

- Étant donné que le titre est renseigné, quand j'enregistre la tâche, alors elle est créée et apparaît dans ma liste.
- Étant donné que le titre est vide, quand j'essaie d'enregistrer, alors un message m'indique quoi corriger et aucune tâche vide n'est créée.

**Priorité :** haute. **Sprint :** 1.

### US-02 — Afficher les tâches

**Histoire.** En tant que personne qui utilise GestiTâches, je veux voir mes tâches dans une liste, afin de savoir ce qu'il me reste à faire.

**Critères d'acceptation**

- Étant donné qu'il existe des tâches, quand j'ouvre la liste, alors chaque tâche affiche au moins son titre et son état.
- Étant donné qu'aucune tâche n'existe, quand j'ouvre la liste, alors un message simple m'invite à en ajouter une.

**Priorité :** haute. **Sprint :** 1.

### US-03 — Consulter une tâche

**Histoire.** En tant que personne qui utilise GestiTâches, je veux ouvrir une tâche, afin d'en relire les détails sans encombrer la liste.

**Critères d'acceptation**

- Étant donné qu'une tâche figure dans la liste, quand je la sélectionne, alors son titre, sa description, sa date d'échéance et son état sont présentés.
- Étant donné qu'une tâche demandée n'existe pas, alors l'application indique qu'elle est introuvable plutôt que d'afficher des détails erronés.

**Priorité :** moyenne. **Sprint :** 1.

### US-04 — Modifier une tâche

**Histoire.** En tant que personne qui utilise GestiTâches, je veux corriger le titre ou la description d'une tâche, afin que son contenu reste utile.

**Critères d'acceptation**

- Étant donné une tâche existante, quand j'enregistre de nouvelles informations valides, alors la tâche affiche les changements.
- Étant donné que le titre devient vide, alors l'application refuse l'enregistrement et explique le problème.

**Priorité :** moyenne. **Sprint :** 2.

## Sprint 2 — Gérer et retrouver ses tâches

### US-05 — Marquer une tâche comme terminée

**Histoire.** En tant que personne qui utilise GestiTâches, je veux marquer une tâche comme terminée, afin de distinguer ce qui est fait de ce qui reste à faire.

**Critères d'acceptation**

- Étant donné une tâche en cours, quand je la marque comme terminée, alors son état terminé est visible dans la liste.
- Étant donné une tâche terminée, quand je la rouvre, alors je peux la remettre en cours.

**Priorité :** haute. **Sprint :** 2.

### US-06 — Supprimer une tâche

**Histoire.** En tant que personne qui utilise GestiTâches, je veux supprimer une tâche dont je n'ai plus besoin, afin de garder ma liste à jour.

**Critères d'acceptation**

- Étant donné une tâche existante, quand je confirme sa suppression, alors elle n'apparaît plus dans la liste.
- Étant donné que je ne confirme pas la suppression, alors la tâche reste disponible.

**Priorité :** moyenne. **Sprint :** 2.

### US-07 — Ajouter une date d'échéance

**Histoire.** En tant que personne qui utilise GestiTâches, je veux associer une date d'échéance à une tâche, afin de savoir quand m'en occuper.

**Critères d'acceptation**

- Étant donné une date valide, quand j'enregistre une tâche, alors cette date est conservée et affichée avec la tâche.
- Étant donné que je ne choisis pas de date, alors je peux tout de même enregistrer une tâche sans échéance.

**Priorité :** moyenne. **Sprint :** 2.

### US-08 — Filtrer les tâches selon leur état

**Histoire.** En tant que personne qui utilise GestiTâches, je veux afficher toutes les tâches, seulement celles en cours ou seulement celles terminées, afin de retrouver rapidement ce que je cherche.

**Critères d'acceptation**

- Étant donné une liste qui contient des tâches dans plusieurs états, quand je choisis un filtre, alors seules les tâches correspondantes sont affichées.
- Quand je reviens au filtre « Toutes », alors toutes les tâches réapparaissent.

**Priorité :** basse. **Sprint :** 2.
