# Magical Taruruuto-kun — Traducción al castellano

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/mega-drive/magical-taruruuto-kun)**.

Traducción al español de España de **Magical Taruruuto-kun**, el juego de plataformas de Game Freak publicado por Sega para Mega Drive en 1992. El parche se aplica directamente a la versión japonesa original.

La descarga contiene únicamente el parche. Necesitas tu propia copia del juego.

## Estado

**[v1.0 — Guion e interfaz en castellano](https://github.com/johanderohan/magical-taruruuto-kun-traduccion-es/releases/tag/v1.0)** · 2026-09-19

| Parte | Estado |
|---|---|
| Guion | 65 páginas únicas traducidas desde el japonés: 43 de escenas y 22 de conversaciones durante las fases |
| Títulos de capítulo | Los cuatro traducidos |
| Interfaz | Jugar, Ajustes, controles, música, sonido, voces, selección de magia, marcador y continuación |
| Hechizos | Invisibilidad, ¡Mimora! y Partir en dos |
| Otros gráficos | Fin de partida y señal de dirección «Sigue» |
| Créditos | Funciones del equipo y rótulo de voces traducidos; nombres originales conservados |
| Caracteres | Tildes, ñ, ü, ¡ y ¿ |
| Logotipo | Se conserva el título grande japonés original |
| Partida completa | Pendiente de validación de principio a fin |

### Comprobaciones

Las seis escenas principales y las seis conversaciones diferentes se han ejecutado en **Genesis Plus GX, mediante libretro en Linux x86-64**. Se han revisado sus 65 páginas y comprobado la correspondencia entre el guion y los datos reinsertados. La tabla de encuentros contiene además un alias de cinco páginas; no se cuenta dos veces como contenido nuevo.

Se han comprobado el arranque, el título, Ajustes, los cuatro capítulos, el inicio de las fases, el menú sin hechizos y con los tres disponibles, el marcador, Fin de partida, la pantalla de continuación, los créditos y el final. Para alcanzar todas las escenas y habitaciones se ha usado selección de escenas o de nivel durante las pruebas; esos cambios de depuración no están en el parche.

El título grande japonés se ha comparado píxel a píxel con el original. El parche se ha reaplicado a la ROM japonesa y el resultado coincide byte a byte con la ROM preparada. Se mantiene la comprobación de integridad del juego y se actualizan su checksum y tamaño de cartucho.

**Límites de la revisión:** no se acredita una partida completa, una prueba en consola física ni la cobertura de todas las variantes de juego. Se conservan las voces japonesas, los nombres propios, las marcas y los avisos legales originales. Si encuentras un problema, abre una incidencia e indica la fase, el texto y el emulador utilizado.

## Cómo aplicar el parche

1. Descarga **magical_taruruuto_kun_es_v1.0.xdelta** de [Releases](https://github.com/johanderohan/magical-taruruuto-kun-traduccion-es/releases).
2. Prepara una copia propia de la ROM japonesa original, sin otros parches ni cabecera adicional.
3. Comprueba estos datos:

| ROM de origen | Valor |
|---|---|
| Archivo de referencia | `Magical Taruruuto-kun (Japan).gen` |
| Tamaño | 524.288 bytes (512 KiB) |
| CRC32 | `F11060A5` |
| MD5 | `f676dfdd836199352f105465905c25de` |
| SHA-256 | `dfeff1b64e372b91fd795c73cd5574f23401d5aa34395df2ce034e225011cd2f` |

La extensión puede ser `.gen`, `.md` o `.bin`; lo que debe coincidir es el contenido y su hash.

4. Aplica el archivo con [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o con `xdelta3`:

```bash
xdelta3 -d -s "Magical Taruruuto-kun (Japan).gen" \
  magical_taruruuto_kun_es_v1.0.xdelta \
  "Magical Taruruuto-kun (Castellano).gen"
```

5. Comprueba la ROM resultante:

| Resultado v1.0 | Valor |
|---|---|
| Tamaño | 1.048.576 bytes (1 MiB) |
| MD5 | `2ff6b93de57dc8a4b9f1a0aac4a5ed5a` |
| SHA-256 | `2cb647adf2cd22b2841e2fe1b45dba11985c75570b892f220daa74eb906a64a1` |
| SHA-256 del parche | `7f37d4bed3710bea81c97d6d18e6b96bbcf94127c69f6d06f1328994ba4e29b3` |

6. Inicia una partida nueva. Los estados instantáneos creados con otra ROM pueden contener tablas y gráficos antiguos.

Cada versión debe aplicarse sobre la ROM japonesa original. Se mantiene la región japonesa del cartucho.

## Criterios de traducción

El guion se ha extraído de la ROM japonesa y contrastado con sus pantallas y con el [manual oficial de Sega](https://www.sega.jp/mdmini2/assets/manual/pdf/JP_Magical-Taluluto.pdf). Se ha preparado una biblia de voces y términos, con revisión del sentido, los tratamientos y la maquetación.

Castellano de España, trato de tú, humor infantil y frases naturales. Taru conserva su muletilla «¿Taru?»; Honmaru es expresivo y algo presumido; Mimora habla con cariño a Taru y con ironía a Honmaru. Se mantienen las dudas del original y no se añaden insultos. Las letras y los signos españoles se dibujan con una fuente adaptada de 8×16 píxeles.

| Original | Traducción o grafía fijada |
|---|---|
| タル | Taru |
| 本丸 | Honmaru |
| じゃば夫 | Jabao |
| 原子 | Harako |
| いよな | Iyona |
| ミモラ / りあ | Mimora / Ria |
| たまみえ | Tamamie |
| ライバ～ | Raibar |
| いじがわ / おおあや | Ijigawa / Oaya |
| とうちゃん / にるる | Papá / Niruru |
| どわっは大王 | rey Dowahha |
| 魔法の国 | Reino Mágico |
| 絵本のせかい | mundo de los cuentos |
| すけるるる～ | Invisibilidad: protege temporalmente de enemigos y pinchos |
| ミ～モ～ラ～ | ¡Mimora!: llama a Mimora para atacar a los enemigos en pantalla |
| まっぷたつ!! | Partir en dos: ataque en línea recta |

## Créditos del parche

Proyecto de **[johanderohan](https://github.com/johanderohan)**. Traducción, adaptación gráfica y herramientas preparadas con asistencia de IA y revisión independiente del guion y del reinserto.

La investigación pública de [tryphon77/mtk-multilingual](https://github.com/tryphon77/mtk-multilingual) permitió contrastar direcciones y formatos de los recursos. Este parche parte de la ROM japonesa; utiliza su propio guion castellano y un reinserto mediante pares de letras que conserva el dibujado original de los diálogos. Tipografía adaptada de [DejaVu](https://dejavu-fonts.github.io/).

## Aviso

Traducción de aficionados, sin ánimo de lucro y sin relación con Game Freak, Sega ni los titulares de Magical Taruruuto-kun. No se distribuye la ROM. Los derechos del juego y de sus personajes pertenecen a sus titulares.
