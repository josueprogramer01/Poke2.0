# Poke2.0

Poke2.0 es una aplicación que funciona como un Pokédex interactivo, diseñada para identificar y mostrar información sobre Pokémon utilizando la API [PokeAPI](https://pokeapi.co/). Además, incluye características interactivas que aprovechan el GPS del dispositivo.

## Funcionalidades

1. **Mostrar Pokémon al azar mediante GPS**:
   - La aplicación utiliza el GPS para detectar el desplazamiento del usuario.
   - Cada vez que el usuario se desplace 10 metros, el dispositivo vibrará y mostrará una alerta de "¡Pokémon encontrado!".
   - La alerta incluirá la información de un Pokémon seleccionado al azar desde la API, incluyendo su nombre, imagen y cualquier dato adicional que desees mostrar.

2. **Mostrar Pokémon al azar mediante botón**:
   - Un botón llamado "Mostrar Pokémon" permite al usuario obtener información de un Pokémon al azar sin depender del desplazamiento.
   - Al presionarlo, la aplicación consulta la API para recuperar los datos del Pokémon y los muestra en pantalla.

## Requisitos

- Dispositivo con GPS habilitado.
- Conexión a internet para consumir la API.
- Sistema operativo Android.

## Tecnologías y Librerías Utilizadas

- **Lenguaje**: Java
- **API**: [PokeAPI](https://pokeapi.co/)
- **Patrón de Arquitectura**: MVVM (Model-View-ViewModel)
- **Librerías Sugeridas**:
  - Retrofit o Volley para consumo de la API.
  - LiveData y ViewModel para la arquitectura MVVM.
  - FusedLocationProviderClient para obtener la ubicación del usuario.
  - Vibrator para activar la vibración en el dispositivo.
  - Glide o Picasso para cargar imágenes desde URLs.

## Instalación y Ejecución

1. **Clona este repositorio**:

   ```bash
   git clone https://github.com/tu-usuario/Poke2.0.git
   ```

2. **Abre el proyecto en Android Studio**:
   - Asegúrate de tener configurado el SDK de Android.

3. **Configura permisos**:
   - En el archivo `AndroidManifest.xml`, asegúrate de incluir los permisos necesarios:
     ```xml
     <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
     <uses-permission android:name="android.permission.INTERNET" />
     <uses-permission android:name="android.permission.VIBRATE" />
     ```

4. **Ejecuta la aplicación**:
   - Conecta tu dispositivo Android o usa un emulador.
   - Compila y ejecuta la aplicación desde Android Studio.

## Detalles Técnicos

- **Interfaz**:
  - Diseño amigable y responsivo utilizando componentes nativos de Android y Material Design.
  - Pantalla principal que muestra la información del Pokémon encontrado o generado.

- **GPS y Alerta**:
  - El desplazamiento del usuario es calculado en tiempo real utilizando el GPS.
  - Cada 10 metros, se activa un evento que muestra la alerta y recupera un Pokémon.

- **Consumo de API**:
  - La API de PokeAPI es consultada para obtener información de Pokémon de manera eficiente y en tiempo real.

## Próximas Mejoras

- Implementación de un historial de Pokémon encontrados.
- Animaciones adicionales al mostrar la información del Pokémon.
- Mejora del manejo de errores y estado sin conexión.

## Contacto

Si tienes preguntas o sugerencias, no dudes en contactarme:

- **Autor**: [Josue Alvarez Rodriguez](mailto:arj1931126@gmail.com)
- **GitHub**: [TuUsuario](https://github.com/tu-usuario)


