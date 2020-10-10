---
description: >-
  Un rolereact permet à vos membres d'obtenir eux-même un rôle en cliquant sur
  une réaction.
---

# RoleReact

## Créer le rolereact <a id="create"></a>

Pour créer le rolereact, vous avez le choix entre trois méthodes :

{% hint style="warning" %}
Peu importe la méthode que vous choisissez, le rolereact devra être sur un message de **DraftBot**.
{% endhint %}

* **Simple message:** `say [message]`  La commande say permet d'envoyer un simple message Discord.

{% hint style="info" %}
Vous pourrez modifier ce message dans le futur avec la commande `say [Identifiant du message].`
{% endhint %}

* **Embed automatique:** `rolereact create [Titre de l'embed]`  Cette solution vous permet à ce que l'embed soit modifié lors de l'ajout ou le retrait d'un rôle dans le rolereact. À la fin, cela ressemble à cela : 

![R&#xE9;sultat d&apos;un rolereact utilisant un embed automatique](../.gitbook/assets/image%20%2810%29.png)

* **Embed personnalisé:** `embed` ou [depuis le panel web](https://www.draftbot.fr/dashboard) dans l'onglet **Embeds** de votre serveur. Cette méthode vous permet de créer un embed totalement personnalisable à votre goût.  Voici un exemple de cette méthode :  

![R&#xE9;sultat d&apos;un rolereact utilisant un embed personalis&#xE9;](../.gitbook/assets/image%20%289%29.png)

{% hint style="info" %}
Vous pourrez modifier l'embed dans le futur depuis le panel web.
{% endhint %}

## Ajouter un rôle à un rolereact <a id="add"></a>

Pour ajouter à un rôle à un rolereact, il vous suffit d'utiliser la commande `rolereact add [Identifiant du message de DraftBot]`

{% hint style="warning" %}
Pour obtenir l'identifiant d'un message, vous devez au préalable activer le mode développeur dans les paramètres utilisateur dans **Apparence** ou **Comportement** suivant votre appareil.   
  
Il vous suffira ensuite de **laissé appuyer votre doigt** sur le message si vous êtes sur téléphone ou de faire **clique droit** sur le message si vous êtes sur ordinateur puis ensuite de sélectionner **Copier l'identifiant**.
{% endhint %}

Ensuite, DraftBot vous demandera quel rôle doit être ajouté. Vous pouvez donner le nom du rôle ou le mentionner, les deux solutions fonctionnent.

{% hint style="danger" %}
Pour que le rolereact fonctionne, DraftBot doit posséder au moins un rôle qui est au dessus du grade que vous souhaitez ajouter au rolereact.
{% endhint %}

Et pour finir, DraftBot vous demandera quel emoji doit être cliquer pour obtenir ce rôle, il vous suffit de l'écrire.

{% hint style="info" %}
Si vous souhaitez ajouter un autre rolereact au même message, il vous suffit de répéter la même opération.
{% endhint %}

## Supprimer un rôle à un rolereact <a id="delete"></a>

Pour supprimer un rôle d'un rolereact, il vous suffit d'utiliser la commande `rolereact remove [Identifiant du message de DraftBot]`

{% hint style="warning" %}
Pour obtenir l'identifiant d'un message, vous devez au préalable activer le mode développeur dans les paramètres utilisateur dans **Apparence** ou **Comportement** suivant votre appareil.   
  
Il vous suffira ensuite de **laissé appuyer votre doigt** sur le message si vous êtes sur téléphone ou de faire **clique droit** sur le message si vous êtes sur ordinateur puis ensuite de sélectionner **Copier l'identifiant**.
{% endhint %}

DraftBot vous demandera ensuite quel emoji du rôlereact doit être supprimé, il vous suffit de l'indiquer.

{% hint style="info" %}
Si vous souhaitez supprimer un autre rolereact du même message, il vous suffit de répéter la même opération.
{% endhint %}

## Configurer un rolereact <a id="config"></a>

Vous pouvez configurer un rolereact vous permettant ou non à ce que la réaction du membre soit supprimé après que le membre est obtenu le rôle.   
  
Si vous souhaitez configurer cette option pour un rôlereact, il vous suffit d'utiliser la commande`rolereact config [Identifiant du message de DraftBot]`

* En cliquant sur la réaction ✅, les réactions des membres seront supprimé et ils **ne pourront plus** se retiré le rôle depuis le rolereact.
* En cliquant sur la réaction ❌, les réactions des membres au rolereact seront conservé et **pourront** se retiré le rôle depuis le rolereact.
