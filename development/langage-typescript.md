# TypeScript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'intéret de TypeScript dans l'IDE  ✔️
- les types de bases  ✔️
- comment et pourquoi étendre une interface  ✔️
- les classes et les decorators  ✔️

## 💻 J'utilise

### Un exemple personnel commenté  ✔️

`import { Dispatch } from "react";
import { NavigateFunction } from "react-router";
import { toast } from "react-toastify";
import { ICar } from "../../interfaces/Car";
import { axiosInstance } from "../api";


export const getUserVehicles = async (
  setUserVehicles?: Dispatch<Array<ICar>>,
  setFavoriteUserVehicles?: Dispatch<Array<ICar>>,
  navigate?: NavigateFunction
) => {
  return await axiosInstance
    .get("/accounts/vehicles")
    .then((response) => {
      if (response.status === 200) {
        setFavoriteUserVehicles && setFavoriteUserVehicles(response.data.favorites);
        setUserVehicles && setUserVehicles(response.data.availables);
      }
      return response.data;
    })
    .catch((error) => {
      navigate && navigate("/voiture");
      toast.error("Echec de la récupération du détail de vos véhicules, réesayez plus tard");
      return null;
    });
};
`

### Utilisation dans un projet ❌ 

[lien github](...)

Description :

### Utilisation en production si applicable❌ 

[lien du projet](...)

Description :

### Utilisation en environement professionnel  ✔️

Description :  J'ai utilisé react  / typescript / react-native pendant 6 mois a ma précédente entreprise. 

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
