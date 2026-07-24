# Notas operativas — asistente Caferini

Convenciones para las corridas automatizadas (Trello + repo) del asistente
operativo de Caferini. Mantener este archivo al día cuando cambien.

## Notas/ideas en tarjetas de Trello

El servidor MCP de Trello conectado no expone lectura ni escritura de
comentarios de tarjeta (no hay acción "comment" en ninguna herramienta
`trelloRead*`/`trelloWrite*`). Como sustituto, las notas o ideas del agente
se agregan al final de la **descripción** de la tarjeta, precedidas por una
línea `---` y el prefijo `[AGENTE]`, conservando todo el contenido previo.
Así queda claro qué texto escribió una persona y qué texto agregó el agente.

Ejemplo:

```
(descripción original de la tarjeta, sin tocar)

---
[AGENTE] texto de la idea/consulta/aviso del agente.
```

Si en algún momento se agrega una herramienta real de comentarios de Trello
al servidor MCP, migrar a comentarios nativos en vez de este parche.
