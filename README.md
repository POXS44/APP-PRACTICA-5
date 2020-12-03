# APP-PRACTICA-5


### Tarea 1.1: Crear y explorar el proyecto 


<img src="img\1.JPG"/>
<img src="img\2.JPG"/>

### Explorando el editor de diseño

### Tarea 1.2: Agregar elementos Views en el editor de Layout

Se crea el diseño de la interfaz de usuario para la aplicación HelloToast en el editor de
diseño mediante las características ConstraintLayout. Puede crear las restricciones
manualmente, como se muestra más adelante, o automáticamente mediante la herramienta
Conexión automática.

### -Examinar las restricciones (constraint) de los elementos

#### Abra activity_main.xml desde el panel Proyecto > Android si aún no está abierto. Si la pestaña Design (diseño) aún no está seleccionada, haga clic en ella.
<img src="img\3.JPG"/>

####  -Si no hay ningún blueprint, haga clic en el botón Select design surface de la barra de herramientas (puede presionar la tecla B, para cambiar entre cada modo) y elija Design + blueprint
<img src="img\4.png"/>

#### -La herramienta Conexión automática también se encuentra en la barra de herramientas. Está habilitado de forma predeterminada. Para este paso,asegúrese de que la herramienta no está deshabilitada

<img src="img\4.JPG"/>

#### Haga clic en el botón de acercar para acercar los paneles de diseño y blueprint para ver de cerca.


#### -Seleccione TextView en el panel del árbol de componentes (Component tree).

#### -El "Hello World" se resalta en los paneles de diseño y blueprint y las restricciones para el elemento TextView son visibles.

<img src="img\5.JPG"/>

#### -A continuación, se muestra como establecer una restricción o constraint con el contenedor padre al lado derecho del TextView

<img src="img\6.JPG"/>

### Añadir un botón al layout
Cuando está habilitada, la herramienta Conexión automática crea automáticamente dos
+ más restricciones para un elemento de interfaz de usuario en el diseño primario.
Después de arrastrar el elemento al diseño, crea restricciones basadas en la posición del
elemento.

Comience con una pizarra limpia. El elemento TextView no es necesario, por lo
que mientras está seleccionado, pulse la tecla Supr + elija Edición > Eliminar.
Ahora tiene un diseño completamente en blanco

<img src="img\7.png"/>

Arrastre un botón desde el panel Paleta a cualquier posición de la presentación.
Si coloca el elemento Button en el área media superior de la presentación,
pueden aparecer restricciones automáticamente. Si no es así, puede arrastrar
restricciones a la parte superior, izquierda y derecha del diseño
<img src="img\8.JPG"/>

+ Añada un segundo botón en la parte inferior del layout y del mismo modo cree
las restricciones correspondientes con los elementos próximos a él. 

<img src="img\9.JPG"/>

+ Pruebe borrar todos los constraints o restricciones de un elemento,
seleccionando y pasando el puntero sobre este y seleccionar cleal all
constraints

<img src="img\10.png"/>


### Tarea 1.3: Cambiar los atributos de los elementos de la interfaz de usuario

En esta tarea, ingresa nuevos valores y cambia los valores de los atributos importantes
de Button, que son aplicables a la mayoría de los tipos de vista.

###  Cambiar el tamaño del Button
El editor de layout ofrece controles de cambio de tamaño en las cuatro esquinas de una
view para que pueda cambiar el tamaño de la view rápidamente. Puede arrastrar los
controladores en cada esquina de la View para cambiar su tamaño, pero al hacerlo,
codifica las dimensiones de ancho y alto. Evite la codificación de tamaños para la
mayoría de los elementos de Vista, porque las dimensiones codificadas no se pueden
adaptar a diferentes tamaños de pantalla y contenido.
En su lugar, use el panel Atributos en el lado derecho del editor de layout para
seleccionar un modo de tamaño que no use dimensiones codificadas. El panel Atributos
incluye un panel de tamaño cuadrado llamado inspector de vista en la parte superior. Los
símbolos dentro del cuadrado representan la configuración de alto y ancho:

1. Height Control: Este control especifica el atributo layout_height y aparece en
dos segmentos en los lados superior e inferior del cuadrado. Los ángulos indican
que este control está configurado en wrap_content, lo que significa que la Vista
se expandirá verticalmente según sea necesario para adaptarse a su contenido. El
"8" indica un margen estándar establecido en 8 dp.
2. Width Control: Este control especifica layout_width y aparece en dos
segmentos en los lados izquierdo y derecho del cuadrado. Los ángulos indican
que este control está configurado en wrap_content, lo que significa que la Vista
se expandirá horizontalmente según sea necesario para adaptarse a su contenido,
hasta un margen de 8 dp.
3. Botón de cierre del panel atributos. Haga clic para cerrar el panel


### Siga los siguientes pasos: 

### Seleccione el botón superior en el panel Árbol de componentes.
### Haga clic en la pestaña Atributos en el lado derecho de la ventana del editor de layout.

<img src="img\10.JPG"/>

### Haga clic en el control de ancho las veces que sea necesario; debe lograr el valor match_constraint para el layout_width

<img src="img\11.png"/>

+ Realice la misma modificación para el botón inferior, el resultado es que ambos
botones deben cubrir todo el ancho del constraint.
<img src="img\12.JPG"/>
+ Establezca wrap_content al layout_height, también puede usar un valor fijo
de 16dp


<img src="img\13.JPG"/>


### Siga los siguientes pasos:
+ Después de seleccionar el primer botón, edite el campo ID en la parte superior
del panel Atributos a button_toast para el atributo android: id, que se usa para
identificar el elemento en el layout.

<img src="img\14.JPG"/>

+ Establezca el atributo de background en @color/colorPrimary. (A medida que
ingresa @c, aparecen opciones para una fácil selección). Si no está establecido
el color, hágalo en colors.xml

<img src="img\1.png"/>

<img src="img\15.JPG"/>

+ Establezca el atributo textColor en @android:color/white.

<img src="img\16.JPG"/>

+ Edite el atributo text en Toast.
<img src="img\17.JPG"/>

+ Selecciona el segundo botón y edite su campo id a button_count

<img src="img\18.JPG"/>

+ Edite el atributo text del segundo botón a Contar


<img src="img\19.JPG"/>


+ Cambie el color de texto y de fondo a los botones

<img src="img\20.JPG"/>

###  Agregar el elemento TextView y sus atributos correspondientes

Una habilidad de usar ConstraintLayout es que puedes agregar elementos en cualquier
parte del espacio disponible y establecer sus restricciones con cualquier elemento
próximo al que se está agregando.

+ Desde el panel Palette y el apartado Common, agregue un elemento View
TextView y establezca el atributo id a show_count.

<img src="img\21.JPG"/>

+ Establezca las restricciones del TextView, la parte superior con el botón de Toast
y su parte inferior con el botón contador.

<img src="img\22.JPG"/>

+ Establezca las restricciones izquierda y derecha del elemento TextView al lado
correspondiente al contenedor padre.
<img src="img\23.JPG"/>

+ Establezca el valor text a 0
<img src="img\24.JPG"/>



+ Establezca el valor textSize a 160sp
<img src="img\25.JPG"/>

+ Establezca el textStyle a bold

<img src="img\26.JPG"/>

+ Cambie layout_width y layout_height a match_constraint


<img src="img\27.JPG"/>

+ Establezca el textColor a @color/colorPrimary
<img src="img\28.JPG"/>

+ Establezca un valor preferido al atributo background, opcional el #0F49CD

<img src="img\29.JPG"/>

+ Establezca el valor gravity a center_vertical

<img src="img\31.JPG"/>



### Tarea 1.4: Editando el layout en el XML


¡El diseño de la aplicación Hello Toast está casi terminado! Sin embargo, aparece un
signo de exclamación junto a cada elemento de la interfaz de usuario en el árbol de
componentes (Component Tree). Pase el puntero sobre estos signos de exclamación para
ver los mensajes de advertencia, como se muestra a continuación. Aparece la misma
advertencia para los tres elementos: las cadenas codificadas deben usar recursos.


+ Edite el fichero strings.xml que se encuentra en la carpeta res/values:


<img src="img\32.JPG"/>

### Siga los siguientes pasos:
+ Abra el fichero activity_main.xml y cambie el modo solamente a código
<img src="img\33.JPG"/>

+ Cambie el valor de text del TextView a un @string/count_initial_value
<img src="img\34.JPG"/>

+ Cambie el valor de text del botón superior a @string/button_label_toast

<img src="img\35.JPG"/>

+ Cambie el valor de text del botón inferior a @string/button_label_count

<img src="img\36.JPG"/>


### Tarea 1.5: Agregar el manejador del evento onClick para los botones


+ Establezca el siguiente código al botón que tenga como id button_toast, antes de
cerrarlo

<img src="img\37.JPG"/>


+ Establezca el siguiente código al botón que tenga como id button_count, antes
de cerrarlo

<img src="img\38.JPG"/>
+ Abra el MainActivity.kt y agregue el siguiente código
<img src="img\40.JPG"/>

+ Agregue el siguiente código al método showToast
<img src="img\41.JPG"/>

+ Agregue el siguiente código al método countUp
<img src="img\42.JPG"/>

Muestre la aplicación funcionando con el contador funcionando el contador y el
mensaje Toast mostrándose cada vez que el usuario de Clic

<img src="img\43.JPG"/>
<img src="img\2.png"/>
<img src="img\44.JPG"/>


