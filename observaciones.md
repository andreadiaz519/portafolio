# Comentarios Generales

Andrea, quiero felicitarte por haber terminado tu portfolio! Qué bueno que hayas personalizado los colores para darle tu impronta. Se que ha sido un largo camino el que has recorrido desde el primer día hasta finalizar el proyecto, que te encontraste muchos escoyos en el camino y valoro que hayas salido adelante!

La sección de la cita está preciosa! Me gusta mucho la elección de la imagen, los colores y la frase es muy linda también. Tiene buen espaciado y se ve bien en todas las pantallas.

En cuanto al Responsive, la versión desktop se ve bien aunque hay un detalle de visualización a tener en cuenta: algunos logos en la sección de Conocimientos, se deforman. Esto ocurre porque las imagenes NO son cuadradas y tiene fijado widht y height en valores absolutos que fuerzan a la imagen a adaptarse al formato cuadrado. Con quitar uno de los dos se soluciona. Si tuviera que decidir yo, dejaria solo el height. Los logos se deforman en todas las distintas pantallas.

En el desktop habría que ajustar algunos margenes. Por ejemplo, la navbar se pega a la scroll-bar a la derecha (específicamente el botón de contacto). En la sección de contacto también hay algunas alineaciones que se ven desordenadas, y los placeholders tocan los bordes de los input, estaria bueno ponerle un poco de padding para separarlo del borde. En la misma sección, los íconos de las redes se ven "raros", tienen fondo blanco. Cuidado con el border radius, entiendo que querias que se vean redondos, pero esa propiedad te corta el pajarito de Twitter... si queres conservar el formato, tal vez sería mejor cambiar el ícono por el de X.

En cuanto a los íconos de redes sociales, es tu elección. Te sugiero que trates de usar los logos del mismo estilo. ¿A qué me refiero? Si usas los que tienen esos brillitos, todos deberian ser de ese estilo. En las distintas librerias suelen agruparlos según quien los diseñó, esto permite que tengan cierta coherción y se vea más prolijo. De todas formas esto es una nota personal, no afecta al proyecto en sí, en cuanto a lo académico.

En tablet y mobile necesita algunos ajustes. En tablet los proyectos en la sección Mis Proyectos, queda alineada a la izquierda y esto se siente como si estuviera roto. Algo similar ocurre en la sección de contacto, donde las dos columnas quedan defasadas, desalineadas y da esa misma sensación.

En mobile, el problema es que parece que no está terminado. Se ve el menú hamburguesa, que no funciona como tal. Al clickearlo, oculta la barra de navegación y no se puede volver al menú, salvo que refresquemos la página. A su vez desplaza la barra de navegación, que no debería verse y sí se ve, y también está cortada.
En mobile, en la sección principal, el botón queda desalineado y se ve raro. Entiendo que quisiste hacerlo y no te salió, en ese caso está bien la nota que dejaste en el CSS.
En mobile, en la sección  de contacto, esta muy pegada a la sección anterior y a la siguiente. El form también necesitaría unos ajustes de espaciado.

En cuanto al código, algunas pequeñas observaciones:

* HTML:
  * En la línea 138, tenes una <ul> de los links a tus redes sociales. La estructura HTML está muy bien armada. Pero en cada anchor que tenes dentro de cada li, en su mayoría linkeas las home de los sitios de redes sociales y NO **tu** redes sociales. No se si esto fue adrede o es un error conceptual, porque en los textos pones tus usuarios. Por ejemplo, en Twitter, el atributo lo tenes asi: href="https://x.com/home" y deberia ser href="https://x.com/adizsan". Esto ocurre tanto en la sección de contacto como en el footer. En el caso del href para el email, el error sí es conceptual, porque estas linkeando la web de Outlook, y lo correcto es href="**mailto:**andreadiaz_2308@hotmail.com".

  * En la línea 85, utilizas la etiqueta blockquote pero le agregas un <p> dentro que no es necesario. La etiqueta semántica en sí es para texto que sea una cita.

  * Sólo una imagen tiene el atributo **alt** definido. Este atributo es indispensable en cuanto a la accesibilidad.

  * En el footer, utilizas la tag h3 para poner la firma. La etiqueta h3 es importante para la indexación del SEO, por lo que no es muy conveniente ponerla para ese contenido que no te suma para la indexación si queres conseguir clientes o que el buscador te encuentre como programadora. Si queres usar un heading, te recomiendo que uses h5 o h6 para evitar afectar la indexación.

* En el CSS:  
  * En distintos lugares estas usando widht y max-widht, siendo que definis widht con medidas absolutas. El max-widht (o min-widht) tienen sentido cuando el widht usa medidas relativas, y por lo tanto su tamaño se puede ir a más grande (o más chico) de lo que necesitamos en el ancho de pantalla, entonces le permitimos crecer (o achicarse) hasta la medida que establecemos en max-widht (o min-widht).

  * En textos y títulos estás agregando la propiedad _display: block;_ cuando es el display por default de esos elementos.

* En cuanto a los mensajes de los commits, es importante que sean un poco más descriptivos. Si todos son _"cambios"_, _"más cambios"_, etc. El día que necesites volver sobre los commits por algo en particular, vas a tener que revisar uno a uno para encontrarlo. No es necesario que sean super largos, pero por ejemplo si agregaste las imagenes de los conocimientos y pusiste el título y avanzaste con el CSS de esa sección, podes poner algo así: "Sección Conocimientos: Agrego imagenes, titulo y estilado.". Es conciso pero también descriptivo para tener una idea de qué contiene ese commit sin tener que revisarlo entero en su contenido.

Buen trabajo, ¡A seguir aprendiendo!

## Nota final: 7 (siete)

### Nota desagregada:

✅ Estructura correcta de documento HTML
✅ Respeta la consigna
✅ Respeta el diseño dado
❌ Responsive funciona correctamente

✅ Buena estructura de proyecto
✅ Código bien indentado
✅ Comentarios que permiten mejorar la legibilidad del código

✅ Uso correcto de etiquetas semánticas
✅ Buenos nombres de clases

✅ Código CSS estructurado
❌ Utiliza variables CSS

❌ Cumple con criterios básicos de accesibilidad
❌ Reutilización de estilos
❌ Commits con mensajes adecuados
❌ Cuenta con un favicon
❌ Cuenta con etiquetas para redes sociales

❌ ✅