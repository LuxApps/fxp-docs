<h1>Mise en place du connecteur MS Graph:</h1>

<h2>Ajout de l’App registration</h2>

Se rendre sur le portail Azure https://portal.azure.com/

Chercher et se rendre sur "App registrations"

<img src="/assets/img/app_registrations.png" alt="App registrations">

Cliquer sur «New registration»:

<img src="/assets/img/new_registration.png" alt="New registration">

Remplir le nom et sélectionner «Accounts in this organizational directory only (<yourTenant> only - Single tenant)»

<b>Une fois l’app enregistrée, copier et nous envoyer l’Application ID:</b>

<img src="/assets/img/clients/app_graph_id.png" alt="App graph id">

<h2/>Ajout du certificate secret</h2>

Se rendre dans «Certificates and secrets» dans le menu de gauche, cliquer sur«Clients secrets» et sur «New client secret»:

Sélectionner une date d’expiration à 24 mois(Veiller à bien noter la date d’expiration afin de créer un nouveau client secret le moment venu et nous le communiquer avant expiration de l’ancien):

<b>A cette étape il faut bien copier et nous envoyer la « Client Secret Value», elle ne sera plus disponible par la suite:</b>


<img src="/assets/img/clients/certificate.png" alt="Certificate">

<h2>Ajout des permissions</h2>

Se rendre dans «API permissions» dans le menu de gauche, puis cliquer sur «Add a permission»:

<img src="/assets/img/permission.png" alt="Permission">

Sélectionner «Microsoft Graph»:

<img src="/assets/img/microsoft_graph.png" alt="Microsoft Graph">

Sélectionner «Application permissions»:

<img src="/assets/img/app_permissions.png" alt="App Permissions">

Chercher les droits voulus grâce à la barre de recherche:

<img src="/assets/img/search_app_permissions.png" alt="Search App Permissions">

Pour l’import et la mise à jour des utilisateurs:

<ul>
    <li>Ajouter la permission «Group.Read.All»</li>
    <li>Ajouter la permission «User.Read.All»</li>
</ul>

Pour valider les droits ajoutés:

Cliquer sur «Grant admin consent for <yourTenant>» au dessus du tableau:

<img src="/assets/img/grant_admin_consent.png" alt="Grant admin consent">
