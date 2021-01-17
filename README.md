# practices-gmeiko

## 1. Ux - Ui - 20 puntos (GitBranch: feature/front ux)

- Explique brevemente qué son los Mockups y para qué son usados.
  > Los mockups permiten representar como se visualizará la interfaz de una aplicación web o móvil. Define fuentes, colores y posición de los elementos. Esto permite depurar ideas sin necesidad de llevarlas al código, ahorrando tiempo, costos y detectando posibles fallas en la usabilidad de la aplicación.
- Diseñe Mockups para un Login a una plataforma Web (puede realizarlos a mano alzada). Ver ENLACE:

https://drive.google.com/file/d/1veHgZRT3XOAUOpxsRLj8WnlbyTI5WwZD/view?usp=sharing - Ejemplo!
[Ver Mockups](https://drive.google.com/file/d/1veHgZRT3XOAUOpxsRLj8WnlbyTI5WwZD/view?usp=sharing)

- Qué aplicación usaría para implementar los Mockups y por qué. Sea breve.

  > Adobe Xd, se pueden compartir enlaces para los Stakeholders y para los desarrolladores, con especificaciones de colores y assets. Además recibir feedback sobre los flujos dentro de la app. Ejemplo:

  https://xd.adobe.com/view/47d917e4-4cf3-40c1-a29b-e3cd70405ddc-128a/ - Ejemplo!
  [VER](https://xd.adobe.com/view/47d917e4-4cf3-40c1-a29b-e3cd70405ddc-128a/)

## 2. CSS - 20 puntos (GitBranch: feature/front css)

- Diseñe un arquitectura CSS (no es necesario realizar implementación en código):

https://drive.google.com/file/d/1gFyw95kAaJmdkWzisAb2G0n6BFAKBbh4/view?usp=sharing - DISEÑO!
[VER DIAGRAMA](https://drive.google.com/file/d/1gFyw95kAaJmdkWzisAb2G0n6BFAKBbh4/view?usp=sharing)

• Qué preprocesador usaría: SASS, LESS, STYLUS, etc.

> Tengo experiencia con SASS

- Comente el manejo del hack important.
  > Se utiliza para eliminar la lectura natural de los estilos (jerarquía y especificidad), o sea aplica por sobre la jerarquía, el atributo declarado con important.
- Incluya manejo de Themes.

  > Para manejar Themes en angular el archivo principal styles.scss, debe declarar cada tema como una variable y aplicarse en el componente de mayor nivel.

- Describa brevemente su diseño, el por que y técnicas o patrones usados.
  > Esta distribución permite tener mayor control sobre los cambios en los estilos, tiene abstracción, respeta la asignación de responsabilidades, además de ofrecer escalabilidad y mantenibilidad.

## 3. Arquitectura en Angular 6+ - 20 puntos (GitBranch: feature/front angular arq)

- Diseñe una arquitectura de dos capas (no es necesario realizar implementación en código):
  App: módulos de la aplicación
  Store: estado de la aplicación

  > Se realiza pensando en una app que consume la api de Spotify

https://drive.google.com/file/d/1CpW79zLxvsgxqFfOB2cRDrXc_tkshrEY/view?usp=sharing - VER DIAGRAMA!
[VER DIAGRAMA](https://drive.google.com/file/d/1CpW79zLxvsgxqFfOB2cRDrXc_tkshrEY/view?usp=sharing)

-Describa brevemente su diseño, el por qué y técnicas o patrones usados.

> Capa de presentación (Verde claro): Se separan en módulos todas las posibles páginas o urls que pueda navegar el usuario, con la finalidad de que puedan cargarse utilizando Lazy Load. En otro directorio se organizan componentes de presentación que pueden ser compartidos por los diferentes componentes o páginas de la aplicación, respetando la arquitectura de componentes y delegando la responsabilidad de comunicarse con los STORE al componente de mayor nivel.

> Para la capa de datos (Gris): se implementa el patrón REDUCER, con Redux, quien se encargará de la administración y consistencia del estado dentro de toda la aplicación.
