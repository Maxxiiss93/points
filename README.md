# Panel de inversiones

Panel web de solo lectura que muestra en un solo lugar saldos y tenencias de IOL más los montos cargados a mano de otras apps.

- `index.html`: sitio estático de un solo archivo. No necesita build ni variables de entorno.
- Backend: proyecto de Supabase `points` (tablas `inv_*` y Edge Function `iol-sync`).
- Las credenciales de IOL viven como secretos en Supabase, nunca en este repo.

Etapa 1: el panel consulta y no envía órdenes de compra ni de venta.
