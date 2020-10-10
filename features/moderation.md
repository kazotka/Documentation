---
description: >-
  Cette catégorie de commandes vous permet de modérer au mieux votre serveur
  Discord.
---

# Modération

## Permissions des commandes

{% hint style="warning" %}
Cette liste regroupe les **principales commandes** de modération de DraftBot pouvant être utile à vos modérateurs.  
Vous pouvez cependant donner la permission à un rôle d'utiliser ces commandes malgré qui n'a pas la permission requise en utilisant la commande [`roleperms`](roleperms.md) !
{% endhint %}

| Commandes | Permissions requises par défaut |
| :--- | :---: |
| ban/tempban/unban | Bannir des membres |
| mute/tempmute/unmute | Gérer les messages |
| kick | Expulser des membres |
| warn/unwarn | Gérer les messages |
| sanctions \(interface de modération\) | Gérer les messages |
| sanction \(afficher les sanctions\) | Gérer les messages |

## Sanctionner un membre

### Interface de sanction

Vous pouvez sanctionner un membre avec la commande `sanction <membre>`  
Vous obtiendrait alors cette interface : 

![Interface de mod&#xE9;ration avec la commande sanction](../.gitbook/assets/image%20%2822%29.png)

Il vous restera plus qu'à sélectionner la réaction correspondante à la sanction que vous souhaitez infliger au membre.  

### Bannir un membre

Vous pouvez bannir un membre avec la commande `ban` ou alors `tempban` si vous souhaitez bannir temporairement le membre.  
  
Si vous souhaitez retirer le bannissement d'un membre par la suite, vous pouvez le débannir avec la commande `unban` ou depuis l'onglet Bannissement de votre serveur Discord.

### Avertir un membre

Vous pouvez avertir un membre avec la commande `warn <Membre> <Raison>`  
Le membre recevra un message privé avec le motif de son avertissement.  
  
Si vous voulez retirer un avertissement d'un membre avec la commande `unwarn`  
L'avertissement sera retirée de la commande `sanction`

### Rendre muet un membre

Vous pouvez rendre muet un membre avec la commande `mute` ou `tempmute` si la sanction est temporaire.  
  
Vous pourrez, si vous le souhaitez, retirer le mute de cette personne avec la commande `unmute`

Pour plus d'informations concernant ce type de sanction ainsi que sa configuration, vous pouvez vous rendre sur l'article dédié au mute: 

{% page-ref page="mute.md" %}

## Voir les sanctions

Vous pouvez voir les sanctions effectuées sur votre serveur avec la commande `sanction`

{% hint style="info" %}
Vous pouvez compléter cette commande par un pseudo ou une mention pour voir les sanctions d'une personne précise.
{% endhint %}

<table>
  <thead>
    <tr>
      <th style="text-align:center"><code>sanctions</code> sans argument</th>
      <th style="text-align:center"><code>sanctions</code> &lt;Membre&gt;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center">
        <p></p>
        <p>
          <img src="../.gitbook/assets/image (26).png" alt/>
        </p>
      </td>
      <td style="text-align:center">
        <p></p>
        <p>
          <img src="../.gitbook/assets/image (28).png" alt/>
        </p>
      </td>
    </tr>
  </tbody>
</table>

## Supprimer les liens d'invitations Discord

DraftBot vous offre la possibilité que les membres qui ne sont pas Administrateur sur votre serveur et qui postent des invitations Discord qu'elles soient supprimées automatiquement.  
  
Pour activer cette fonctionnalité, il vous suffit de faire la commande `admininvites`

{% hint style="warning" %}
Les personnes qui ont la permission Administrateur de votre serveur sont immunisés par cette fonctionnalité.
{% endhint %}

## Interdire certains mots

Vous pouvez, avec DraftBot, lorsque certains mots sont écrits, qu'il soit remplacée par des caractères spéciaux avec la commande `filter`

![Exemple d&apos;un mot interdit remplac&#xE9; par des caract&#xE8;res sp&#xE9;ciaux](../.gitbook/assets/image%20%2825%29.png)

Pour activer le filter, il suffit de faire la commande `filter on`  
Vous pouvez ensuite ajouter des mots au filter avec la commande `filter add <mot>`

{% hint style="info" %}
Vous pouvez ajouter plusieurs mots en une seule commande en mettent une virgule entre chaque mot.  
Exemple: mot1, mot2, mot3, mot4
{% endhint %}

{% hint style="warning" %}
Le filter se déclenchera uniquement pour les personnes qui **ne sont pas** Administrateur.
{% endhint %}


