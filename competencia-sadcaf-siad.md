# Hoops EC (Carolinazo) frente a SADCAF y SIAD

**Fecha:** 6 oct 2026 · **Pregunta:** ¿qué diferencia, solución o reemplazo ofrece nuestra plataforma ([carolinazo.integroecuador.com](https://carolinazo.integroecuador.com/)) frente a [SADCAF](https://sadcaf.com/torneos/ecuador/todas-subzonas) y [SIAD de Por Fin Deportes](https://siad.porfindeportes.com/siadweb/com.siad.wconsultabarrial)?

> **Cómo se hizo:** el entorno de investigación no pudo abrir directamente sadcaf.com, siad.porfindeportes.com ni la web del Carolinazo, porque el proxy de red los bloqueaba. Lo que se dice aquí sobre SADCAF y SIAD sale de buscadores, fichas de las tiendas de apps, páginas públicas de ligas que usan esos sistemas y sus reglamentos. Lo que se dice de nuestra plataforma sale del documento interno "¿Qué es Hoops EC?". Lo que no se pudo confirmar va marcado como **(por verificar)**.

---

## 1. Respuesta corta

- **Hoy no los reemplazamos.** SADCAF y SIAD son **sistemas de administración de ligas permanentes**. Llevan la afiliación de jugadores, la calificación, los carnets, las sanciones y los traspasos temporada tras temporada, y atienden a decenas de ligas a la vez. Hoops EC es hoy una **plataforma para un evento**, un torneo abierto de baloncesto, y está muy bien resuelta para ese caso.
- **Ya somos mejores en algo concreto: el baloncesto.** SADCAF es casi solo de fútbol, incluido el indor. SIAD es multideporte (fútbol, básquet y ecuavoley), pero genérico y con tecnología GeneXus. Ninguno de los dos muestra una **planilla de vocalía FIBA que funcione sin conexión**, ni una **cuenta propia para cada jugador con consentimiento del representante**, ni una **experiencia para aficionados y auspiciantes** como la nuestra.
- **El reemplazo posible:** convertirnos en *"el SADCAF del baloncesto"*, es decir, el sistema de ligas y torneos de básquet de Ecuador (ligas barriales de básquet, academias, clubes, torneos abiertos e intercolegiales). Para eso nos faltan módulos concretos de liga permanente, que se detallan en la sección 5.

---

## 2. Qué es cada sistema

### SADCAF: "Sistema de Administración de Campeonatos de Fútbol"
- **Quién lo hace:** SADCAF Technology, una empresa ecuatoriana. Las apps están publicadas a nombre de Jhonny y Roger Achig.
- **Para quién:** ligas deportivas barriales y parroquiales, sobre todo en Quito, y ligas de indor fútbol. Entre las que lo usan están Liga Barrial y Parroquial Ciudad de Quito, Turubamba de Monjas La Ecuatoriana, El Sodiro, San Juan, El Condado, San José de Billivaro, Sierra Hermosa, Andrés de Santa Cruz, San Pedro de Tingo, Orquídeas y La Ofelia (indor).
- **Modelo:** **multi-liga**. Cada liga tiene su propio subdominio (`liga.sadcaf.com`, `liga.sadcaftorneos.com` o `liga.sadcaf.com.ec`) y existe un directorio nacional de torneos por zona y subzona.
- **Funciones que se pudieron comprobar:**
  - Inscripciones web: el dirigente carga los datos del equipo y de los jugadores.
  - Calificación de jugadores a cargo de la Comisión de Calificación de la liga, que también legaliza carnets, traspasos e inscripciones.
  - **Carnet de jugador con código QR.** Las ligas cobran entre USD 1 y 1,25 por carnet según sus reglamentos.
  - Lista de jugadores calificados generada por la plataforma, que se presenta para jugar.
  - **Vocalía** de cada partido descargable en PDF.
  - Resultados, tablas, estadísticas en tiempo real, informes finales y búsqueda web de jugadores.
  - Repositorio de reglamentos y documentos de cada liga.
  - Apps para Android e iOS: **SADCAF App** para el público y las ligas, y **SADCAF My Team** para los dirigentes.
- **Se presenta como** "la plataforma líder para la administración de campeonatos de fútbol en Ecuador".
- **Precio:** no está publicado **(por verificar)**.

### SIAD de Por Fin Deportes
- **Quién lo hace:** Por Fin Deportes, de Quito, que también organiza campeonatos barriales, entre ellos **campeonatos nacionales barriales de baloncesto**. El sistema está hecho con **GeneXus**: lo delatan los paquetes `com.genexus.siadapp` y `com.artech.kbsiad` y las URLs `servlet/com.siad.*`.
- **Para quién:** ligas barriales, asociaciones de ligas parroquiales y federaciones cantonales. Una de las consultas públicas se llama "Cantonal SDT", probablemente Santo Domingo de los Tsáchilas **(por verificar)**.
- **Modelo:** jerárquico **región → sector → institución (club) → disciplina → jugador**.
- **Funciones que se pudieron comprobar:**
  - **Consultas públicas** de jugadores por cédula o nombre, con liga, club, disciplina y **fechas de afiliación y calificación**. La consulta "barrial" de la URL que nos pasaron pertenece a esa familia.
  - **Multideporte:** fútbol, básquet y ecuavoley recreativos.
  - App **SIAD 2.0**, gratuita, versión 3.1 de marzo de 2025: calendario, resultados, tabla de posiciones, **sanciones**, **goleadores**, **vocalías en línea**, notificaciones por sector y estadísticas de gestión.
  - Registro de actas de partido **para elaborar las actas de sanción**, que es el flujo disciplinario.
- **Precio:** no está publicado **(por verificar)**.

### Hoops EC (Carolinazo Basquetero)
- Web oficial del torneo, en producción. Usa Next.js y React, InsForge para la base de datos y el login, y está alojada en Hostinger.
- **Un evento:** XI edición con 261 inscripciones de equipos, 18 categorías y 43 grupos, desde U10 hasta +60.
- **Roles:** aficionado, jugador, delegado, vocalía, árbitro y organizador.
- **Funciones diferenciales:** planilla FIBA **sin conexión** (reloj, tiempos muertos, cambios y faltas), cierre del partido por el árbitro con su cédula, QR de inscripción, fixture cargado desde Excel, planillas en PDF, reglas por categoría (por ejemplo, la de juveniles en +50), aprobación del representante para menores, banner de auspiciantes y equipo favorito con cuenta regresiva.

---

## 3. Comparativa de funciones

Leyenda: ✅ lo tiene · ⚠️ parcial o limitado · ❌ no lo tiene · ❓ no se pudo comprobar

| Capacidad | SADCAF | SIAD | **Hoops EC hoy** |
|---|:-:|:-:|:-:|
| Deporte principal | Fútbol e indor | Fútbol, básquet y ecuavoley | **Baloncesto** |
| Varias ligas u organizaciones en una plataforma | ✅ subdominio por liga | ✅ jerarquía región/sector | ❌ un solo torneo |
| Liga permanente (temporadas, varios campeonatos al año) | ✅ | ✅ | ❌ |
| Registro histórico del jugador (afiliación y calificación) | ✅ | ✅ | ⚠️ solo inscripción al evento |
| Identidad del jugador ligada a la cédula | ✅ | ✅ | ⚠️ ligada al correo (ver caso SOP-0001) |
| Comisión de calificación: aprobar o rechazar con documentos | ✅ | ✅ | ⚠️ el organizador aprueba usuarios |
| **Carnet digital con QR** | ✅ | ❓ | ❌ (el QR es para inscribirse, no es carnet) |
| Traspasos o pases entre clubes | ✅ | ❓ | ❌ |
| **Sanciones** (tarjetas o faltas acumuladas, suspensiones, actas) | ❓ | ✅ | ❌ |
| Consulta pública de jugador o sanción por cédula | ✅ | ✅ | ⚠️ búsqueda de jugadores |
| Inscripción web por el dirigente o delegado | ✅ | ❓ | ✅ |
| Cuenta propia del jugador y consentimiento para menores (LOPDP) | ❓ | ❓ | ✅ **diferencial** |
| Vocalía o planilla digital | ✅ PDF | ✅ "en línea" | ✅ **FIBA y sin conexión** |
| Reglas propias del baloncesto (faltas personales y de equipo, tiempos muertos, cuartos) | ❌ | ⚠️ genérico | ✅ **diferencial** |
| Cierre del resultado por el árbitro con su cédula | ❓ | ❓ | ✅ |
| Fixture, resultados y tablas | ✅ | ✅ | ✅ |
| Goleadores o estadísticas individuales | ✅ | ✅ | ❓ (no consta) |
| Cobros (inscripción, carnets, multas) | ⚠️ las ligas cobran por fuera | ❓ | ❌ |
| App nativa con notificaciones | ✅ Android e iOS, dos apps | ✅ Android | ❌ (web) |
| Repositorio de reglamentos y documentos | ✅ | ❓ | ❌ |
| **Auspiciantes y monetización del evento** | ❌ | ❌ | ✅ **diferencial** |
| Experiencia del aficionado (equipo favorito, cuenta regresiva) | ⚠️ | ⚠️ | ✅ **diferencial** |
| Tecnología y experiencia de uso | Web y apps NativeScript | GeneXus (servlets, interfaz antigua) | Next.js moderno |
| Vínculo con una academia (formación → competencia) | ❌ | ❌ | ✅ potencial con Hoops Academy |

---

## 4. Dónde ya les ganamos

1. **Somos nativos del baloncesto.** La planilla FIBA, el control de faltas, los tiempos muertos, los cambios y el reloj son exactamente lo que un vocal de básquet necesita. SADCAF no atiende baloncesto, y SIAD lo atiende con el mismo esquema que el fútbol.
2. **La vocalía funciona sin conexión.** En parques y canchas barriales la señal es mala. Es un argumento de venta fuerte y fácil de demostrar.
3. **El resultado se cierra con firma del árbitro.** Hay trazabilidad de quién validó el marcador, y eso reduce disputas.
4. **Cumplimos con la protección de datos.** Cada jugador tiene su cuenta y el representante aprueba en el caso de menores. Esto encaja con la Ley Orgánica de Protección de Datos Personales de Ecuador, cuyo régimen sancionatorio ya está vigente. Las ligas que manejan miles de cédulas de menores van a necesitarlo.
5. **El evento genera ingresos.** El banner de auspiciantes por niveles (hoy todos en Aliado) convierte la plataforma en una fuente de ingresos para el organizador, no solo en un gasto. Ni SADCAF ni SIAD lo ofrecen según lo que se encontró.
6. **Tecnología y experiencia de uso modernas.** Frente a SIAD (GeneXus y servlets), la diferencia de experiencia se nota a simple vista.
7. **Tenemos un ecosistema propio.** Hoops Academy, con más de 9 sedes, más los torneos permiten seguir a un jugador desde la academia hasta la competencia. Ningún competidor tiene ese canal.

---

## 5. Qué nos falta para ser un reemplazo real

Estos módulos son los que convierten a una liga en cliente recurrente de SADCAF o SIAD. Están ordenados por prioridad:

| Prioridad | Módulo | Por qué |
|:-:|---|---|
| **P0** | **La cédula como identidad única del jugador**, con un representante que gestione a varios menores desde una sola cuenta | Resuelve la causa del caso HOOPS-SOP-2026-0001 (dos jugadoras inscritas desde la misma cuenta) y es como trabajan SADCAF y SIAD |
| **P0** | **Multi-organización**: una plataforma con muchas ligas o torneos, cada uno con su espacio, por ejemplo `liga.hoops.ec` | Sin esto solo podemos vender evento por evento |
| **P0** | **Temporadas y varios campeonatos** por organización, con historial | Las ligas viven todo el año, no un fin de semana |
| **P1** | **Calificación y carnet digital con QR**, verificable en la cancha por el vocal | Es el entregable más visible de SADCAF y una fuente de ingreso por carnet |
| **P1** | **Sanciones**: faltas técnicas y antideportivas, expulsiones, suspensiones automáticas por fechas, actas y consulta pública | Es el núcleo de SIAD y un requisito disciplinario de cualquier liga |
| **P1** | **Estadísticas individuales**: puntos, rebotes, asistencias y faltas por jugador, máximos anotadores | En baloncesto pesan más que en fútbol y la planilla FIBA ya recoge los datos |
| **P2** | Traspasos o pases entre clubes, con reglas de la liga | Hace falta para ligas formales |
| **P2** | Cobros: inscripciones, carnets y multas, al inicio con registro manual (igual que en el software de la academia) | Cierra la parte administrativa |
| **P2** | Repositorio de reglamentos y documentos por liga | Es fácil de hacer y las ligas lo esperan |
| **P2** | Web instalable (PWA) con notificaciones, en lugar de una app nativa | Iguala a SADCAF y SIAD sin publicar dos apps |
| **P3** | Jerarquía federativa (federación → liga → club) y otras disciplinas | Solo si se decide competir fuera del baloncesto |

---

## 6. Posicionamiento recomendado

**"Hoops: la plataforma para ligas y torneos de baloncesto en Ecuador."**

- **No competir con SADCAF en fútbol.** Allí tiene muchas ligas, tiempo en el mercado y efecto red.
- **Competir con SIAD en básquet,** donde nuestra planilla FIBA, el funcionamiento sin conexión y la experiencia de uso son claramente superiores. Por Fin Deportes organiza campeonatos barriales de baloncesto. Puede ser **competidor o aliado** (integración o licencia) y conviene explorarlo.
- **Segmentos objetivo, por orden:**
  1. Torneos abiertos de básquet (como el Carolinazo).
  2. Ligas barriales que tienen disciplina de básquet.
  3. Academias y clubes, con Hoops Academy como cliente cero.
  4. Torneos intercolegiales y universitarios.
- **Mensaje frente a cada uno:**
  - *Frente a SADCAF:* "Ellos hacen fútbol. Nosotros hacemos baloncesto de verdad: planilla FIBA, estadísticas por jugador y vocalía sin conexión."
  - *Frente a SIAD:* "La misma administración de liga, con una experiencia moderna, cuentas por jugador conformes a la protección de datos y auspiciantes que financian tu torneo."

---

## 7. Pendiente de verificar

1. **Precios** de SADCAF y SIAD: cuánto paga una liga por temporada o por carnet, y qué parte del cobro de USD 1–1,25 por carnet queda para SADCAF.
2. Si SADCAF ofrece **módulo de sanciones** y si SIAD emite **carnet con QR**.
3. Si SIAD tiene **planilla específica de básquet** (faltas personales y de equipo).
4. Cuántas ligas o deportistas usa cada uno, para dimensionar el mercado. Como referencia, Quito tiene unas 300 ligas barriales con alrededor de 450.000 deportistas, y FEDENALIGAS publica 7 federaciones cantonales, 71 ligas, 516 clubes y 13.717 deportistas activos.
5. Una revisión directa de ambos sistemas desde un navegador sin restricciones: capturas, flujo de inscripción y planilla.

---

## Fuentes

- SADCAF: [sadcaf.com.ec](https://sadcaf.com.ec/), [Servicios](https://sadcaf.com.ec/services/), [Acerca de](https://sadcaf.com.ec/about/), [Torneos en Ecuador](https://sadcaf.com/torneos/ecuador/todas-subzonas), [Facebook](https://www.facebook.com/sistema.SADCAF/), [X](https://x.com/sadcaf?lang=es)
- Apps SADCAF: [SADCAF (Google Play)](https://play.google.com/store/apps/details?id=org.nativescript.SadcafApp&hl=en_US), [SADCAF My Team](https://play.google.com/store/apps/details?id=com.sadcaf.myteam&hl=en), [SADCAF App (App Store)](https://apps.apple.com/ec/app/sadcaf-app/id1630773829), [AppAdvice](https://appadvice.com/app/sadcaf/1481354728), [Desarrollador en Google Play](https://play.google.com/store/apps/dev?id=5102655771635046082&hl=es)
- Ligas que usan SADCAF: [Ciudad de Quito](https://ciudaddequito.sadcaf.com/inscripciones), [La Ecuatoriana](https://laecuatoriana.sadcaf.com/inscripciones), [El Sodiro](https://sodiro.sadcaf.com/inscripciones), [San Juan](https://sanjuan.sadcaf.com/equipo-registrado), [Billivaro](https://billivaro.sadcaf.com.ec/inscripciones), [El Condado](https://elcondado.sadcaftorneos.com/inscripciones), [Reglamento Orquídeas](https://orquideas.sadcaf.com/documentos/reglamento.pdf?cache=1783534460), [Reglamento Andrés de Santa Cruz](https://andresoleary.sadcaf.com/documentos/reglamento.pdf?cache=1782542367), [Reglamento San Pedro de Tingo](https://sanpedrotingo.sadcaf.com/documentos/documento_21.pdf), [Reglamento Sierra Hermosa](https://sierrahermosa.sadcaftorneos.com/documentos/reglamento.pdf?cache=1780011176), [Vocalía La Ofelia](https://ofelia.sadcaf.com/vocalia/pdf/1679/juventud-del-valle-vs-club-deportivo-d.n.c?cache=1787184378)
- SIAD: [Consulta barrial](https://siad.porfindeportes.com/siadweb/com.siad.wconsultabarrial), [Consulta de jugadores](https://siad.porfindeportes.com/siadweb/servlet/com.siad.wconsultajugcal01), [Asociación de Ligas Parroquiales](https://siad.porfindeportes.com/siadweb/servlet/com.siad.wconsultajugcal02), [Cantonal SDT](https://siad.porfindeportes.com/siadweb/servlet/com.siad.wconsultajugcal03), [Login SIAD](https://siad.porfindeportes.com/siadweb/servlet/com.siad.wwpbaseobjects.seclogin), [SIAD 2.0 (Google Play)](https://play.google.com/store/apps/details?id=com.genexus.siadapp&hl=en), [SIAD 2.0 (APKCombo)](https://apkcombo.com/siad-2-0/com.genexus.siadapp/), [Por Fin Deportes (Facebook)](https://www.facebook.com/Porfindeportes/)
- Contexto: [FEDENALIGAS](https://fedenaligas.com/), [Ligas barriales de Quito](https://zonales.quito.gob.ec/?page_id=71449)
