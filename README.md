# GeoIDs

🇬🇧 Consistent identifiers for geographical levels • 🇫🇷 Identifiants cohérents pour niveaux géographiques


## Problem • Problème

🇬🇧 There is no standard for identifiers of geographical levels. We need it to deal with multiple projects ([geozones](https://github.com/etalab/geozones), [geohisto](https://github.com/etalab/geohisto), [udata](https://github.com/opendatateam/udata), [inspire](https://github.com/etalab/inspire) to name a few).

🇫🇷 Il n’y a pas de standard pour les identifiants des niveaux géographiques. Nous en avons besoin pour certains projets ([geozones](https://github.com/etalab/geozones), [geohisto](https://github.com/etalab/geohisto), [udata](https://github.com/opendatateam/udata), [inspire](https://github.com/etalab/inspire), etc.).


## Solution

🇬🇧 Use the given pattern for each geographical level:

```
{country_code}:{geographical_level}:{code}@{start_date}
```

Where:

* `country_code` is a 2-letter country code
* `geographical_level` is the localised level
* `code` is the standard code for that place
* `start_date` is the date when that place was set at the [ISO 8601 extended format](https://en.wikipedia.org/wiki/ISO_8601#Calendar_dates) `YYYY-MM-DD`

🇫🇷 Utiliser le motif suivant pour chaque niveau géographique :

```
{code_pays}:{niveau_geographique}:{code}@{date_debut}
```

Où :

* `code_pays` est le code pays à 2 caractères
* `niveau_geographique` est le niveau traduit sans accents
* `code` est le code standard pour cet endroit
* `date_debut` est la date de création de cet endroit au [format étendu ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Calendar_dates) `AAAA-MM-DD`


## 🇫🇷 Exemples

* Pour la région Bretagne : `fr:region:53@1970-01-09`
* Pour le département de l’Ain : `fr:departement:01@1860-07-01`
* Pour la collectivité d’outre-mer de Saint-Martin : `fr:collectivite-outre-mer:978@2007-02-21`
* Pour la commune d’Aranc : `fr:commune:01012@1942-01-01`
