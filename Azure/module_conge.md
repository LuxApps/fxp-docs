<h1>Activation de la synchronisation des congés avec le calendrier des salariés :</h1>

<h2>Récupération du Tenant ID</h2>

Se rendre sur <a href="https://portal.azure.com">Le portail Azure</a>

Chercher et cliquer sur Tenant properties:

<img src="/assets/img/tenant_properties.png" alt="Tenant properties">

<b>Copier et nous envoyer le “Tenant ID”:</b>

<img src="/assets/img/tenant_id.png" alt="Tenant id">

<h2>Ajout de l’App registration</h2>

Chercher et se rendre sur "App registrations"

<img src="/assets/img/app_registrations.png" alt="App registrations">

Cliquer sur «New registration»:

<img src="/assets/img/new_registration.png" alt="New registration">

Remplir le nom et sélectionner «Accounts in this organizational directory only (<yourTenant> only - Single tenant)»

<b>Une fois l’app enregistrée, copier et nous envoyer l’Application ID:</b>

<img src="/assets/img/app_graph_id.png" alt="App graph id">

<h2/>Ajout du certificate secret</h2>

Se rendre dans «Certificates and secrets» dans le menu de gauche, cliquer sur«Clients secrets» et sur «New client secret»:

<img src="/assets/img/certificate.png" alt="Certificate">

Remplir une description et sélectionner une date d’expiration à 24 mois(Veiller à bien noter la date d’expiration afin de créer un nouveau client secret le moment venu et nous le communiquer avant expiration de l’ancien):

<img src="/assets/img/secret.png" alt="Secret">

<b>A cette étape il faut bien copier et nous envoyer la « Client Secret Value», elle ne sera plus disponible par la suite:</b>

<img src="/assets/img/secret_value.png" alt="Secret value">

<h2>Ajout des permissions</h2>

Se rendre dans «API permissions» dans le menu de gauche, puis cliquer sur «Add a permission»:

<img src="/assets/img/permission.png" alt="Permission">

Sélectionner «Microsoft Graph»:

<img src="/assets/img/microsoft_graph.png" alt="Microsoft Graph">

Sélectionner «Application permissions»:

<img src="/assets/img/app_permissions.png" alt="App Permissions">

Ajouter la permission « Calendars.ReadWrite » grâce à la barre de recherche :

Cliquer sur « Grant admin consent for <yourTenant> » :

Pour valider les droits ajoutés:

Cliquer sur «Grant admin consent for <yourTenant>»:

<img src="/assets/img/grant_admin_consent.png" alt="Grant admin consent">

