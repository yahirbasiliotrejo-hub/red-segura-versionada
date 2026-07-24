# Reglas básicas de firewall

## Reglas permitidas

| Origen | Destino | Puerto | Acción | Justificación |
|---|---|---|---|---|
| LAN escolar | Internet | 80 | Permitir | Navegación web |
| LAN escolar | Internet | 443 | Permitir | Navegación segura |
| IP administrativa | Servidor académico | 22 | Permitir | Administración remota autorizada |

## Reglas denegadas

| Origen | Destino | Puerto | Acción | Justificación |
|---|---|---|---|---|
| Cualquier origen | Servidor académico | 22 | Denegar | Evitar fuerza bruta |
| Cualquier origen | Cámara IP | 80 | Denegar | Evitar acceso no autorizado |
| Red invitados | Red administrativa | Todos | Denegar | Separación de red |

## Recomendación

No exponer servicios críticos a redes externas.
