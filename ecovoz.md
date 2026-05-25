# Challenge

<p style="font-size: 150%; font-weight: bold; color: #279B48; padding-bottom: 0;">Proyecto EcoVoz: Asistente Verde de la Comunidad</p>

**ODS 12: Producción y Consumo Responsables**

¿Te has preguntado cuántos residuos generamos diariamente en nuestra escuela? En este tutorial, construirás una aplicación con MIT App Inventor que utiliza Inteligencia Artificial para permitir a los usuarios interactuar mediante comandos de voz y clasificar la basura de su entorno.

*Nota: Para optimizar el tiempo de nuestra sesión de 90 minutos, utilizaremos el Mockup visual que ya se encuentra diseñado en tu pantalla. Nos enfocaremos al 100% en la programación lógica de los bloques.*

# Setup

## Inyectando componentes de hardware e IA

Para que nuestra aplicación pueda escuchar y responder de manera autónoma, necesitamos agregar componentes no visibles de procesamiento de lenguaje natural y sensores físicos.

Sigue los pasos a continuación para preparar tu entorno de desarrollo:

1. Dirígete a la **Paleta** del lado izquierdo de tu pantalla.
2. Abre el cajón de **Medios (Media)** y arrastra al visor el componente `ReconocimientoDeVoz` (SpeechRecognizer).
3. En el mismo cajón de Medios, selecciona y arrastra el componente `TextoAVoz` (TextToSpeech).
4. Ahora, ve al cajón de **Sensores** y arrastra al visor un `Vibrador` (Vibrator).

Verás que estos elementos se posicionarán en la parte inferior del teléfono bajo la sección de *Componentes no visibles*.

# Simple EcoVoz Tutorial

## Programación del "Camino Feliz"

Ahora haz clic en el botón de **Bloques** en la esquina superior derecha para iniciar la programación estructurada que le dará vida a la IA.

Cuando **Boton_Microfono** sea cliqueado:
* Llama al **ReconocimientoDeVoz** para activar el hardware del micrófono y capturar el comando de audio del usuario.

Cuando el **ReconocimientoDeVoz** regrese con el texto de lo escuchado:
* Integra una estructura condicional `si... entonces`.
* Evalúa: Si el texto del resultado contiene la palabra clave **"plástico"**, entonces:
    * Llama al **Vibrador** para generar una alerta háptica de 500 milisegundos.
    * Cambia la imagen central del visor por el contenedor de reciclaje azul.
    * Llama al componente **TextoAVoz** para que la app dicte el consejo: *"El plástico tarda 500 años en degradarse. Deposítalo en el contenedor azul."*

# Expand Your App

## ¡El Reto de Imaginación Autónoma! (45 minutos)

Ya dominas la estructura base de la comunicación por voz. Ahora es momento de aplicar el enfoque de la Nueva Escuela Mexicana para resolver un problema crítico de tu entorno escolar de manera independiente.

**Tu misión:** Modifica y expande el código de tus bloques para que tu asistente sea capaz de reconocer al menos **3 situaciones críticas o residuos diferentes** de tu plantel (por ejemplo: *'orgánico', 'papel', 'fuga de agua', 'luz encendida'*).

Condiciones obligatorias para cumplir el reto con éxito:
* Cada palabra clave debe provocar una respuesta de voz (TextoAVoz) totalmente diferente, persuasiva o alarmante según la gravedad de la situación.
* La interfaz visual del teléfono debe cambiar de forma drástica (colores de fondo o imágenes de alerta) para cada caso detectado.
* Configura un patrón de vibración único en los bloques para diferenciar los residuos o reportes más peligrosos.
