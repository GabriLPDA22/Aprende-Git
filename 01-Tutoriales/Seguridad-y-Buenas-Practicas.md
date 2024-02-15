# Seguridad y Buenas Prácticas en Git 🛡️

Mantener la seguridad y seguir buenas prácticas son aspectos cruciales del trabajo con Git y el desarrollo de software en general. Este capítulo cubre recomendaciones esenciales para proteger tu código y optimizar tu flujo de trabajo.

## Seguridad en Git

### Uso de HTTPS y SSH

- **HTTPS** es recomendado para usuarios ocasionales de Git, proporcionando una forma segura de transferir información entre tu repositorio y tu máquina local.
- **SSH** ofrece una alternativa más segura para usuarios frecuentes y proyectos que requieren un nivel adicional de seguridad.

### Autenticación de Dos Factores (2FA)

Activar 2FA en plataformas como GitHub, GitLab, o Bitbucket añade una capa extra de seguridad, protegiendo tu cuenta de accesos no autorizados.

## Buenas Prácticas

### Commits Atómicos

Realiza commits pequeños y específicos que representen un único cambio lógico. Esto facilita la revisión de código y la localización de errores.

### Mensajes de Commit Claros y Descriptivos

Escribe mensajes de commit que expliquen claramente qué cambios se han realizado y por qué. Sigue convenciones como:

- Comenzar el mensaje con una línea resumen corta, seguida de una descripción más detallada si es necesario.
- Usar el modo imperativo: "Añade" en lugar de "Añadido".

### Revisión de Código

Participar en revisiones de código no solo mejora la calidad del código sino que también fomenta el aprendizaje y la colaboración entre el equipo.

### Mantener las Dependencias Actualizadas

Las dependencias desactualizadas pueden ser una fuente significativa de vulnerabilidades de seguridad. Usa herramientas como Dependabot en GitHub para mantener tus proyectos actualizados.

## Herramientas de Seguridad

- **Git-secrets** y **truffleHog** son herramientas que pueden ayudar a prevenir la filtración de información sensible, como claves API y contraseñas, al escanear el historial de commits en busca de patrones que se asemejen a datos confidenciales.

- **Significado de Commits con GPG**: Configura Git para firmar tus commits con GPG, lo que proporciona verificación de autoría y asegura que los cambios provienen de una fuente confiable.

```bash
git config --global user.signingkey TU_CLAVE_GPG
git commit -S -m "Tu mensaje de commit"
```

---

Siguiendo estas pautas y utilizando las herramientas adecuadas, puedes mejorar significativamente la seguridad y la eficacia de tu flujo de trabajo en Git. 🌟
