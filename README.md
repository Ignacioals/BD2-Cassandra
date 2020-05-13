# BD2-Cassandra

#### DB creation
* Start cassandra from the shell, and copy the content in `CargaDeDatos.txt` to it

#### Querys
1. Get the bands that are in a user's playlist. Copy the following text into the shell `select * from tabla1 where id_usuario = 5 ;`

2. Get the autor from a specific song. Copy the following into the shell:
* by the song name `select id_cancion, nombre_cancion, letra_cancion, id_autor_letra, apellido_autor_letra, nombre_autor_letra from tabla234 where nombre_cancion = 'Battery' allow filtering;`
* by the song id `select id_cancion, nombre_cancion, letra_cancion, id_autor_letra, apellido_autor_letra, nombre_autor_letra from tabla234 where id_cancion = 5 allow filtering;`

3. Get the autor that is owner of the lyrics and the melody from the same song. Copy the following into the shell `select id_cancion, nombre_cancion, letra_cancion, id_autor_letra, apellido_autor_letra, nombre_autor_letra, id_autor_musica, apellido_autor_musica,nombre_autor_musica from tabla234 where nombre_cancion = 'Holy Diver'  allow filtering;`

4. Get the albums from a record company. Copy the following into the shell `select id_discografica, nombre_discografica, id_album, nombre_album, ano_album from tabla578 where id_discografica=1 allow filtering ;`

5. Get the reviews for a specific song in all albums. Copy the following into the shell `select id_resena, id_autor_resena, apellido_autor_resena,nombre_autor_resena, fecha_resena, texto_resena from tabla6 where id_canciones contains 15 ;`

6. Get the name of all the songs in an album. Copy the following into the shell `select id_album, nombre_album, id_cancion, nombre_cancion from tabla578 where id_album = 5 allow filtering;`

7. Get the albums that have a specific song. Copy the following into the shell `select id_album, nombre_album, ano_album, portada_album from tabla578 where id_cancion = 3 allow filtering;`
