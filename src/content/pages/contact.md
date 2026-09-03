---
title: Contactez-moi
description: Page de contact pour me joindre directement.
noIndex: false
hideTOC: false
draft: false
---
> [!info]
> Remplissez ce formulaire pour m'envoyer un message. Je vous répondrai dans les plus brefs délais.


<!--
  Ce formulaire fonctionne nativement avec Netlify Forms.
  Déployez votre site sur Netlify, et il sera automatiquement détecté.
  Les soumissions apparaissent dans l'onglet "Forms" de votre tableau de bord Netlify.
  L'action pointe vers /thank-you, inclus avec ce thème.
-->

<form
  name="contact"
  method="POST"
  data-netlify="true"
  netlify-honeypot="bot-field"
  action="/thank-you"
  class="form-sleek"
>
  <!-- Champ piège anti-spam -->
  <input type="hidden" name="bot-field" />

  <!-- Nom du formulaire (requis par Netlify) -->
  <input type="hidden" name="form-name" value="contact" />

  <div class="mb-4">
    <label for="name" class="block mb-2 font-medium">Nom complet</label>
    <input
      type="text"
      id="name"
      name="name"
      required
      class="w-full p-3 border rounded"
      placeholder="Jean Dupont"
      autocomplete="name"
    />
  </div>

  <div class="mb-4">
    <label for="email" class="block mb-2 font-medium">Adresse email</label>
    <input
      type="email"
      id="email"
      name="email"
      required
      class="w-full p-3 border rounded"
      placeholder="votre@email.com"
      autocomplete="email"
    />
  </div>

  <div class="mb-6">
    <label for="message" class="block mb-2 font-medium">Votre message</label>
    <textarea
      id="message"
      name="message"
      rows="5"
      required
      class="w-full p-3 border rounded"
      placeholder="Décrivez votre demande..."
    ></textarea>
  </div>

  <button
    type="submit"
    class="btn btn-primary w-full py-3 text-lg">
    Envoyer le message
  </button>
</form>