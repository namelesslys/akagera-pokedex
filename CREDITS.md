# Image credits

The app's `app.js` wildlife records include `imageCredit`, `imageSource`, and `imageLicense` fields. The current implementation intentionally keeps image attribution alongside the species data so each record can be audited or replaced without changing UI code.

Several images are based on Wikimedia Commons files supplied for this project, including Elephant_JP.jpg, South-western_black_rhinoceros_(Diceros_bicornis_occidentalis)_female.jpg, Giraffe_Gathering_Akagera_National_Park.jpg, Zèbre_dans_la_savane.jpg and Quatre_hippopotames.jpg.

For production distribution, verify every linked Commons file's current author/licence and add the exact attribution text if required by the licence.


## Verified image updates

- Common Warthog — “Common Warthog (Phacochoerus africanus).jpg” by sussexbirder, Wikimedia Commons, CC BY 2.0.
- Common Duiker — “Common Duiker (Sylvicapra grimmia) (6011670419).jpg” by Bernard DUPONT, Wikimedia Commons, CC BY-SA 2.0.
- Waterbuck — “Waterbuck (Kobus ellipsiprymnus).jpg” by sussexbirder, Wikimedia Commons, CC BY 2.0.

These files were selected specifically to avoid ambiguous filename matches. Source pages should be retained with the deployed app for attribution.
