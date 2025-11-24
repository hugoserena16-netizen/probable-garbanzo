
SerHu — Instrucciones para convertir el demo en tienda funcional
===============================================================

Archivos incluidos:
- index.html, products.html, product.html, cart.html, checkout.html
- style.css
- js/app.js
- logo.svg
- img/*.jpg
- products.json

Funcionalidad actual:
- Carrito persistente en localStorage.
- Checkout y "pago con tarjeta" son simulados (no envían datos a ningún servicio).
- Puedes abrir el sitio en cualquier hosting estático (Netlify, Vercel, GitHub Pages).

Cómo conectar pagos reales (resumen):
1) Stripe Checkout (recomendado):
   - Necesitas una cuenta Stripe y un backend sencillo (Node/Express, PHP, etc.) para crear sesiones de Checkout.
   - El frontend redirige al endpoint de Stripe que crea una Checkout Session y devuelve la URL.
   - Documentación: https://stripe.com/docs/payments/checkout

2) PayPal Buttons:
   - Puedes usar las Smart Payment Buttons de PayPal con tu client-id público y callbacks.

3) Alternativa (si usas Shopify):
   - Importa los productos al panel de Shopify y activa pasarelas de pago en Settings > Payments.

Si quieres, puedo generar el código de backend para Stripe (ej. Node.js) y adaptar el frontend para hacer pagos reales. Pídemelo y te lo preparo.
