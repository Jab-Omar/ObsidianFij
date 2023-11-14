---
tags:
  - Windows
date: 2023-11-14
---
# Contourner les Restrictions avec un Proxy

L'utilisation d'un proxy offre la possibilité de contourner diverses restrictions, qu'elles soient d'ordre géographique ou imposées au sein d'un réseau local par des dispositifs tels qu'un pare-feu. Explorons cette démarche à travers un exemple concret.

## 1. Restriction d'Accès à un Site via le Pare-feu

Imaginons que vous souhaitez accéder au site "domaine.xyz", mais votre pare-feu en sortie de réseau bloque cet accès. Dans ce schéma initial, la requête est bloquée par le pare-feu, entravant votre accès au site.

## 2. Contournement de la Restriction via un Proxy Externe

Pour contourner cette restriction, vous pouvez utiliser un proxy externe sur Internet. Ainsi, votre ordinateur va solliciter le proxy pour accéder au site "domaine.xyz", et le proxy renverra les résultats. La requête ne sera pas bloquée, car vous communiquez avec le proxy plutôt qu'avec le site directement. Le schéma résultant illustre cette approche de contournement.


**Remarques importantes :**

- La réussite du contournement dépend de la configuration du pare-feu et éventuellement du proxy utilisé :
    - Un pare-feu peut bloquer des proxies connus utilisés pour contourner les restrictions, en effectuant du filtrage DNS ou de site Web.
    - Certains proxies utilisent des ports spécifiques comme le 3128 ou le 8080. Si le pare-feu n'autorise pas ces ports en sortie vers Internet, la connexion vers le proxy peut échouer.
    - Monter un proxy sur le port 80 (http) ou 443 (https) peut être une stratégie efficace pour utiliser le proxy comme rebond, mais cela dépend également de la configuration du pare-feu.