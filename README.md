He decidido crear en XML una etiqueta raíz llamada usuarios, dentro de la cual estarán los usuarios registrados con los campos que se nos han pedido en la tarea.

En el XSD, he creado un elemento complexType llamado *usuarios*, dentro del cual hay otro elemento complexType llamado *usuario*. Ambos son complejos porque tienen atributos y subelementos.

Sin embargo, el resto de los elementos son de tipo simple, ya que no tienen más de un atributo ni subelementos dentro.

En cuanto a las restricciones, he decidido que el nombre de usuario no puede tener mayúsculas ni caracteres especiales, excepto el carácter "_". El email debe ir en minúsculas y debe contener obligatoriamente un "@", además de tener un mínimo de dos caracteres y un máximo de n caracteres.

El teléfono lo he dividido en el primer número y el resto de los siguientes, debiendo empezar por 6, 7, 8 o 9, que son muchos de los prefijos en España, de forma muy parecida a cómo funciona el código postal.

Por último, he establecido un máximo de 16 caracteres para la contraseña, con el objetivo de evitar crear contraseñas innecesariamente largas.
