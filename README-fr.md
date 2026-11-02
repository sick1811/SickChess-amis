# SickChess – version pour les amis

[English](README.md) | **Français**

Jeu d'échecs pour Windows : contre l'ordinateur (Stockfish 17.1, ou Maia 3 qui joue comme un humain, selon le niveau), à deux sur le même PC ou en ligne entre amis Steam, problèmes, entraînement aux ouvertures et analyse de tes parties.

- **Maia 3, deux modèles :** le petit (5M, 21 Mo, livré avec le jeu) et le grand (79M, 312 Mo, le plus humain). Le jeu prend le grand dès qu'il est là, sauf sur un petit PC, qui garde le petit. [Maia-3 by the CSSLab, University of Toronto](https://github.com/CSSLab/maia3).
- **Tables de finales Syzygy :** toutes les finales de 3 à 5 pièces (940 Mo), pour l'évaluation, les finales et l'apprentissage.

**Installer :** télécharger [SickChess_Installation.exe](https://github.com/sick1811/SickChess-amis/releases/latest/download/SickChess_Installation.exe), le lancer, puis ouvrir SickChess depuis l'icône du Bureau.

- Il faut Internet et environ 2 Go de libre : les problèmes (220 Mo), les tables de finales (940 Mo) et le grand modèle de Maia (312 Mo) se téléchargent pendant l'installation (environ 1,5 Go, une seule fois).
- Aucun droit administrateur n'est nécessaire. Windows demande une fois l'autorisation pour le pare-feu : répondre Oui laisse passer les mises à jour et le jeu en ligne.
- Si Windows affiche « Windows a protégé votre ordinateur » : « Informations complémentaires », puis « Exécuter quand même » (le jeu n'est pas encore signé).

Le jeu se met ensuite à jour tout seul depuis le menu, jamais pendant une partie. Les parties, le profil et les réglages sont gardés.

**Jouer en ligne :** Steam doit être ouvert. Ouvrir SickChess **avant** d'accepter l'invitation d'un ami, ou taper le code du salon. Steam indique « Spacewar » : c'est normal, c'est le numéro de test de Valve en attendant la sortie sur Steam.

**Licences et code source :** SickChess est sous GPL v3 ; le fichier `jeu/maia.py` et [Maia 3](https://github.com/CSSLab/maia3) (CSSLab, Université de Toronto) sont sous AGPL v3 ; Stockfish est sous GPL v3. Le code de chaque version est joint à sa publication (`SickChess_code_source_<version>.zip`, page [Releases](https://github.com/sick1811/SickChess-amis/releases)). Les textes des licences sont livrés avec le jeu (dossier `licenses`, `moteur/COPYING-Stockfish.txt`, `moteur/maia/COPYING-Maia3.txt`).

## Crédits

SickChess repose sur le travail de nombreux projets open source et créateurs. Merci à tous.

**Moteurs d'échecs**
- **[Stockfish 17.1](https://github.com/official-stockfish/Stockfish/tree/sf_17.1)** : joue et analyse les parties. Licence [GPL v3](https://www.gnu.org/licenses/gpl-3.0.html), livré sans modification, comme programme séparé.
- **[Maia-3 by the CSSLab, University of Toronto](https://github.com/CSSLab/maia3)** : l'adversaire « humain », en deux modèles. Licence AGPL v3, utilisé avec l'accord du CSSLab. Article : Monroe et al., « Chessformer: A Unified Architecture for Chess Modeling », ICLR 2026.

**Données**
- **[Problèmes de Lichess](https://database.lichess.org/#puzzles)** : 4 180 151 problèmes, domaine public (CC0).
- **[Ouvertures « chess-openings » de Lichess](https://github.com/lichess-org/chess-openings)** : noms et lignes d'ouvertures, domaine public (CC0).
- **[Tables de finales Syzygy](https://syzygy-tables.info)** : 3, 4 et 5 pièces, [générées par Ronald de Man](https://github.com/syzygy1/tb), librement redistribuables.

SickChess n'est ni affilié à Lichess.org ni approuvé par lui.

**Graphismes, polices et sons**
- **Pièces « Classique »** : d'après les dessins de Colin M. L. Burnett (Cburnett), GPL v2 ou ultérieure.
- **Polices Barlow Semi Condensed, Outfit et JetBrains Mono** : leurs auteurs respectifs, SIL Open Font License 1.1.
- **Bruitages de bois** : pack « Impact Sounds » de [Kenney](https://kenney.nl), domaine public (CC0).
- **Autres pièces, plateaux, logo, fond du menu, carillons et musique « Zugzwang »** : créés pour SickChess, tous droits réservés, comme le nom SickChess.

**Bibliothèques**
- **[python-chess](https://github.com/niklasf/python-chess)** : Niklas Fiekas, les règles du jeu, GPL v3 ou ultérieure.
- **[Pygame](https://www.pygame.org)** : LGPL v2.1. **[SDL2, SDL2_image, SDL2_mixer, SDL2_ttf](https://libsdl.org)** : licence zlib.
- **[numpy](https://numpy.org)** : licence BSD (avec OpenBLAS et LAPACK, BSD). **[ONNX Runtime](https://onnxruntime.ai)** : Microsoft, licence MIT.
- **Python** : Python Software Foundation License. **OpenSSL** : Apache License 2.0.
- **FreeType** : Portions of this software are copyright © The FreeType Project (www.freetype.org). All rights reserved.
- **libjpeg** : This software is based in part on the work of the Independent JPEG Group.
- **libpng, zlib, libtiff, libwebp, libogg, Opus, opusfile, libmodplug, PortMidi, libffi, SQLite** : licences libres, textes complets dans le dossier `licenses`.
- **Steamworks SDK** (`steam_api64.dll`) : © Valve Corporation, redistribué selon l'accord Steamworks SDK.
- **Microsoft Visual C++ Runtime** : composant redistribuable de Microsoft.

Chess, Stockfish, Lichess, Steam et les autres noms cités appartiennent à leurs propriétaires respectifs et sont utilisés uniquement pour les identifier. SickChess est un projet indépendant.

Merci de ne partager ni le jeu, ni le lien, ni les images.
