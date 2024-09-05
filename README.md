# Don Quijote ChatBot


>[!NOTE]
> La plantilla de la interacción de texto fue extraida de [binary-hood](https://github.com/binary-hood/ChatBot-Starter)

Este proyecto es una aplicación de chat que permite a los usuarios interactuar en tiempo real. 
El personaje principal de este chat es Don Quijote de la Mancha, este personaje unico usara su particular experiencia y forma de hablar para responder a tus preguntas.

Utiliza un backend en Python y un frontend en HTML/CSS para ofrecer una experiencia de usuario fluida y atractiva.


## Arquitectura del Software

La arquitectura de la aplicación se compone de lo siguiente:

  - **main/**: Directorio principal que contiene los archivos esenciales del proyecto.
      - **static/**: Contiene archivos estáticos como hojas de estilo CSS.
         - `style.css`: Archivo de estilos para la interfaz de usuario.
      - **templates/**: Contiene las plantillas HTML utilizadas por la aplicación.
         - `chat.html`: Plantilla principal para la interfaz de chat.
      - **.env**: Archivo de configuración para variables de entorno.
      - **.gitignore**: Especifica los archivos y directorios que deben ser ignorados por Git.
      - `app.py`: Archivo principal que ejecuta la aplicación.
      - `prompt.py`: Archivo que gestiona las interacciones y las respuestas del chat.
      - `README.md`: Este archivo, que proporciona información sobre el proyecto.
      - `requirements.txt` Lista de dependencias necesarias para ejecutar la aplicación.
  


## Funciones Principales

- **app.py**
  - Inicia el servidor web y gestiona las rutas de la aplicación.
  - Configura la conexión a la base de datos (si aplica) y maneja las solicitudes de los usuarios.

- **prompt.py**
  - Contiene la lógica para procesar los mensajes de los usuarios y generar respuestas.
  - Utiliza un modelo de lenguaje para ofrecer respuestas coherentes y relevantes.

- **style.css**
  - Define el diseño y la presentación de la interfaz de usuario.
  - Asegura que la aplicación sea visualmente atractiva y fácil de usar.

- **chat.html**
  - Estructura la interfaz de usuario del chat.
  - Incluye elementos interactivos para enviar y recibir mensajes.


## Instrucciones de Instalación

Para instalar y ejecutar la aplicación, sigue estos pasos:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/Yessid-ML/Don_Quijote_chat.git
   cd tu_repositorio
2. Crea un entorno virtual (opcional pero recomendado):
    ```bash
    python -m venv venv
    source venv/bin/activate  # En Linux/Mac
    venv\Scripts\activate  # En Windows
3. Instala dependencias
    ```bash
    pip install -r requirements.txt
4. Configura las variables de entorno
    ```bash
    .env file
5. Ejecuta la aplicacion.
    ```bash
    python app.py



### Ejemplos de Uso
```markdown
## Ejemplos de Uso

Una vez que la aplicación esté en funcionamiento, abre tu navegador y dirígete a `http://localhost:5000` para acceder a la interfaz de chat. Puedes empezar a enviar mensajes y recibir respuestas en tiempo real.


## Instalacion Installation & Setup

[Instalar Python] https://www.dataquest.io/blog/installing-python-on-mac/

[Install pip] https://phoenixnap.com/kb/install-pip-mac

If you have Python & pip installed then check their version in the terminal or command line tools

```
python3 --version
```

```
pip --version
```

## Installing Flask

In your terminal run the requirements.txt file using this pip

```
pip install -r requirements.txt
```

## What you will create

In this tutorial, I will guide you through the process of building a chatbot that can carry out conversations with users using natural language processing.

To start, we will be using Microsoft DialoGPT, a pre-trained language model that can generate human-like responses to given prompts. We will be integrating DialoGPT with Flask, a popular Python web framework, to create a web application that can communicate with users via a chat interface.

For the frontend of our application, we will be using HTML, CSS, and JavaScript to create a visually appealing and interactive chat interface. Additionally, we will be using jQuery to handle the HTTP requests that are made to the backend server.

Throughout the tutorial, I will provide step-by-step instructions on how to set up your development environment, install the necessary dependencies, and create the required files and code for the application. I will also explain how to train and fine-tune the DialoGPT model to improve the accuracy of its responses.

By the end of this tutorial, you will have a fully functional chatbot that can engage in conversations with users, and you will have gained valuable experience in using Microsoft DialoGPT, Flask, and web development technologies such as HTML, CSS, and JavaScript.

# ChatBot Link
The Chatbot is constructed using the Microsoft/DialoGPT-medium model.

```
https://huggingface.co/microsoft/DialoGPT-medium
```

# User-Html

```
var userHtml = '<div class="d-flex justify-content-end mb-4"><div class="msg_cotainer_send">' + user_input + '<span class="msg_time_send">'+ time + 
    '</span></div><div class="img_cont_msg"><img src="https://i.ibb.co/d5b84Xw/Untitled-design.png" class="rounded-circle user_img_msg"></div></div>';
```

# Bot-HTML

```
var botHtml = '<div class="d-flex justify-content-start mb-4"><div class="img_cont_msg"><img src="https://i.ibb.co/fSNP7Rz/icons8-chatgpt-512.png" class="rounded-circle user_img_msg"></div><div class="msg_cotainer">' + bot_response + '<span class="msg_time">' + time + '</span></div></div>';
```