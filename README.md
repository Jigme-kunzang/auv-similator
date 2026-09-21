# Projet : Simulateur de trajectoire (Robotique/Data)

*Estimation : 25 à 40 heures de travail (environ 3 à 5 week-ends)*
*Ce projet est très visuel. Il utilise des bibliothèques C++ reconnues dans la robotique et le calcul scientifique, et montre une maîtrise bas niveau du traitement de données capteurs.*

- Récupération des données GPS (5 à 8h) : Trouver des données open-source de trajectoires animales ou de drones marins (AUV, gliders) et comprendre leur format (CSV ou NetCDF). Lire les fichiers avec rapidcsv (CSV) ou netcdf-cxx4 (NetCDF).

    **Utilisation des données du AUV Autosub6000**

- Nettoyage et traitement (10 à 15h) : Utiliser Eigen pour le calcul matriciel et implémenter un lissage des trajectoires (moyenne glissante, puis filtre de Kalman). Retirer les points GPS aberrants (les "bugs" du capteur sous l'eau) avec des tests de vitesse et de distance entre points, calculés avec GeographicLib.
- Visualisation 3D/Carto (10 à 15h) : Utiliser Matplot++ pour les graphiques 2D, exporter les trajectoires en GeoJSON/KML pour les afficher sur carte (QGIS, Google Earth), et utiliser VTK (ou ParaView) pour la visualisation 3D. Organiser le projet avec CMake et faire une mise en page propre sur GitHub.

Langage utilisé : C++17 (compilation avec CMake)