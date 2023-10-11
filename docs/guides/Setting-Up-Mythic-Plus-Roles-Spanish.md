# Bot de Discord Jeeves: Configurando la Integración de Roles de Mythic Plus (M+)

Con el bot Jeeves para Discord, puedes enriquecer la experiencia de tu servidor asignando roles según el puntaje M+ del jugador para la temporada actual. Así es cómo puedes configurarlo:

## Guía Paso a Paso

1. **Agrega Jeeves a tu Servidor de Discord**: Comienza invitando al bot Jeeves a tu servidor.

2. **Inicia Sesión en el Sitio Web de Jeeves**: Dirígete al sitio web de Jeeves e inicia sesión.

3. **Accede al Panel de Control del Servidor**: Navega al panel de control específico de tu servidor. Desde allí, dirígete a la pestaña _Gestión de Roles_.

4. **Activa la Integración M+**: Dentro de la pestaña de Gestión de Roles, habilita la función `Role Management`. A continuación, activa la `M+ Integration`.

## Configuración de Roles por Defecto

Por defecto, Jeeves proporciona roles basados en los siguientes formatos de nombres:

- `2500+ Mythic Score`
- `2500+ Mythic+ Score`
- `2500 Mythic Score`
- `2500 Mythic+ Score`
- `Below 200`

**Recuerda**: Es necesario que crees manualmente los roles para estos rangos en tu servidor.

## Configuración Personalizada de Roles

Si deseas designar nombres personalizados para los roles:

1. Activa la opción `Custom Role Map` dentro de la página de Integración M+.

2. Especifica el rol que te gustaría asignar en cada rango.

## Proceso de Asignación de Roles

- **Para Nuevos Usuarios**: Después de unirse a tu servidor, los usuarios deben ejecutar el comando `/authorize` o hacer clic en el botón _Authorize_. Una vez que enlacen sus cuentas, Jeeves asignará automáticamente los roles correspondientes en un plazo de 60 segundos.

- **Para Usuarios Existentes**: Si ya han autorizado en el pasado, pueden usar el comando `/roles update`. Esto actualizará sus datos y determinará si califican para una actualización de rol.

**Nota**: Los servidores con estado _Premium_ se benefician de actualizaciones automáticas de datos de personajes y actualizaciones de roles de rutina. Después de la autorización inicial, no son necesarios más comandos.

## Información Importante

- **Conocimiento del Personaje**: Jeeves solo reconoce los personajes disponibles en el momento de la autorización. Cualquier cambio en el nombre o reino de un personaje, o la adición de nuevos personajes, requerirá una reautorización para su detección.

## Consejos Pro

- **Sincronizar Colores de Roles**: Ejecuta `/role-tools mythic-plus sync-colors` para alinear los colores de tus Roles M+ con los tonos actuales de puntuación raiderio.

- **Restablecer Rangos al Final de la Temporada**: El comando `/role-tools mythic-plus reset-ranks` es útil para restablecer el rango de todos al final de cada temporada. Por favor, ten cuidado con este comando y asegúrate de leer su documentación acompañante.
