La estructura está compuesta por:
1. index.pug
2. player.pug (ejemplo: chrispaul.pug)
3. year-all-draft-team.pug (ejemplo: 2005-all-draft-team.pug)
4. position.pug (ejemplo: pg.pug)

La idea sería que en 
player.pug se guarden la información de los jugadores mediante variables
position.pug se importan las variables de los jugadores desde player.pug
year-all-draft-team.pug se importa toda la estructura de position.pug

position.pug sería el maquetado del box-model de cada jugador
year-all-draft-team.pug sería el maquetado del box-model de todos los jugadores juntos en un rectangulo

En position.pug
Lo unico que hay que hacer es hacer el include de player.pug
h3.player-position cambiarlo
class de div en la position adecuada, por ejemplo .pg

------------------------------------
actualización final 1
Ya quedó todo armado. Para cambiar algo solo hay que crear un player.pug e include en position.pug del year-all-draft-team.pug, luego también agregar year-all-draft-team.pug en index.pug