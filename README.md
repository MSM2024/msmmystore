
# MSM MY STORE - msmmystore.com - FINAL V3

Portal revista digital + ecosistema MSM + ELIANA IA oficial selva cascada + ZAFIRO + legal completo + PWA instalable con banderas 🇵🇪🇩🇴🇴🇲🇯🇵

## Stack
Next.js 15 App Router, React 19, TypeScript estricto, Tailwind, Supabase (Postgres, Auth, Storage, RLS), OpenAI para ELIANA, Vercel

## Quick Start en tu computadora
1. pnpm install
2. cp .env.example .env.local y llena claves
3. pnpm dev -> http://localhost:3000

## Deploy Vercel (ver docs/ANALISIS_COMPLETO.md para pasos suaves)
- Importa repo GitHub en Vercel
- Añade env vars
- Domains: msmmystore.com + www.msmmystore.com -> A @ 76.76.21.21 y CNAME www cname.vercel-dns.com

## Estructura
src/app/page.tsx -> Inicio con hero ecosistema
src/app/zafiro -> ZAFIRO
src/app/eliana -> ELIANA oficial selva cascada
src/app/servicios, marketplace, viajes, escuela, etc
src/app/terminos, privacidad, cookies, aviso-legal, accesibilidad
src/app/mi-cuenta -> Perfil VIP
src/app/crear-mi-negocio -> Form 5 pasos
src/app/admin -> Panel edición
supabase/migrations/001_core.sql -> Schema completo con RLS

## Campos editables por Don Miguel en /admin/configuracion
- Correo oficial, dirección legal, horarios, redes, precios, textos legales, imágenes

## ELIANA IA
Endpoint: POST /api/eliana/chat
- Saludo obligatorio Bendiciones
- No pide PIN/CVV/OTP
- Escala con PERSONA o DON MIGUEL
- Rate limiting, Zod validation, server-only

## Legal
Todas las páginas legales con versión, fecha, historial, sin datos inventados.

## PWA
manifest.json + iconos en public/icons + service worker (next-pwa)

## Build check
pnpm lint && pnpm typecheck && pnpm build

## Contacto
MSM My Store LLC - Kissimmee FL USA - +1 (772) 301-5523 - info@msmmystore.com
Alcance: 🇵🇪 Perú 🇩🇴 Dominicana 🇴🇲 Omán 🇯🇵 Japón + USA
