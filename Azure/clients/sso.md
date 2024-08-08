<h1>Mise en place du connecteur SSO</h1>

<h2>Récupération du Tenant ID</h2>

Se rendre sur le portail Azure https://portal.azure.com/

Chercher et cliquer sur Tenant properties:

<img src="/assets/img/tenant_properties.png" alt="Tenant properties">

<b>Copier et nous envoyer le “Tenant ID”</b>

<h2>Ajout de l’Enterprise Application</h2>

Chercher et se rendre sur «Enterprise applications», puis cliquer sur «New application»:

<img src="/assets/img/clients/enterprise_applications.png" alt="Enterprise applications">

Cliquer sur "Create your own application":

<img src="/assets/img/create_application.png" alt="Create application">

<b>Copier et nous envoyer l’”Application ID”:</b>

<img src="/assets/img/clients/application_id.png" alt="Application ID">

Dans l’onglet «Properties», il faut modifier la valeur de «Assignment required» pour mettre «No»:

<img src="/assets/img/clients/properties.png" alt="Properties">

Dans l’onglet «Single sign on», il faut choisir «SAML»:

<img src="/assets/img/saml.png" alt="Saml">

<h2>Configuration du Single sign on</h2

Dans l’onglet Single sign on, il faut éditer la « Basic SAML configuration » comme suit avec les valeurs suivantes :

Identifier : {VotreNomDeDomaine} (Exemple: https://domaine.lu)

Reply URL : {VotreNomDeDomaine}/saml/acs/{ApplicationID} (Exemple: https://domaine.lu/saml/acs/518b88aa-d461-4c31-94ac-bfc6d3bfc3ba)

Sign On URL : {VotreNomDeDomaine}/saml/login

Relay State : {VotreNomDeDomaine}/saml/acs/{AppID}

Logout URL : {VotreNomDeDomaine}/saml/logout

<img src="/assets/img/clients/single_sign_on.png" alt="Single sign on">

<b>Télécharger et nous envoyer le «SAML Signing Certificate» au format Base64 (Veiller à bien noter la date d’expiration afin de créer un nouveau certificat le moment venu et nous le communiquer avant expiration de l’ancien)</b>

<h2>Création d’un groupe d’utilisateurs pouvant se connecter à la plateforme</h2>

Retourner dans «Azure Active Directory»

Chercher et cliquer sur «Groups» dans le menu de gauche:

<img src="/assets/img/groups.png" alt="Groups">

Ajouter un groupe de sécurité via le bouton «New group»

<b>Copier et nous envoyer l’ID du groupe créé</b>

Ajouter les utilisateurs pouvant se connecter à la plateforme au groupe nouvellement créé

Vérifier que les utilisateurs ont bien ces données renseignées :

<ul>
<li>Email</li>
<li>Nom</li>
<li>Prénom</li>
<li>Manager</li>
<li>Société</li>
<li>Equipe</li>
</ul>
