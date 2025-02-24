# 🚀 Slack Interactive Scoreboard
Este proyecto utiliza GitHub Actions para enviar notificaciones automáticas a un canal de Slack cada vez que se agrega una nueva pregunta a través de un push en la rama main o mediante una ejecución manual.

## 📋 Características
- Envía preguntas automáticamente cuando se detectan cambios en questions.yml.
- Permite enviar preguntas manualmente con información personalizada.
- Notificaciones interactivas con títulos, colores y mensajes personalizados.
## ⚙️ Cómo funciona
#### 🔄 Ejecución automática por push
Cada vez que se realiza un push a la rama main que incluya cambios en el archivo questions.yml, se enviará automáticamente una pregunta aleatoria a Slack.

#### 📝 Ejecución manual
Puedes ejecutar manualmente el flujo desde la pestaña de acciones de GitHub con los siguientes parámetros:

- trigger_quiz: Determina si se ejecuta el quiz (Sí o No).
- name: Nombre de quien envía la pregunta.
- question: Pregunta personalizada para enviar.
#### 🔑 Configuración
1. Crea un webhook de Slack:

	- Ve a Incoming Webhooks en Slack.
	- Copia la URL generada.
	
2. Agrega el webhook como un secreto en tu repositorio:
	- Ve a Settings → Secrets and variables → Actions.
	- Crea un secreto llamado SLACK_WEBHOOK y pega la URL.
	
	
## 💬 Únete al canal de Slack
¡Participa en las preguntas y responde en tiempo real con otros miembros del curso! 🚀

- Únete al canal de Slack usando este enlace: [Unirse al canal](https://githubactions-k3n8492.slack.com/archives/C08F46XFL2D) 
🔗
- Asegúrate de estar registrado con el mismo correo que usas en GitHub para recibir notificaciones personalizadas.


## 🚀 Uso


1. Clona el repositorio:
	```
		git clone https://github.com/tu-usuario/tu-repo.git
		cd tu-repo
	```

2. Agrega nuevas preguntas en questions.yml con el formato:
	```
		- ¿Cuál es la capital de Francia?
		- ¿Qué lenguaje se usa en GitHub Actions?`
	```

3. Realiza un push:
	```
		git add questions.yml
		git commit -m "Nueva pregunta añadida"
		git push origin main
	```

¡Mira la notificación en tu canal de Slack! 🎉

## 🤝 Contribuciones
¡Las contribuciones son bienvenidas! Solo haz un fork del repositorio y crea un pull request.