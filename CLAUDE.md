# Centre IA en Marxa — Landing Page

## Stack
- Next.js 14 (App Router) + React + Tailwind CSS
- Un sol fitxer de contingut: `app/page.jsx`
- Deploy: Vercel (auto-deploy des de `main` a GitHub)
- Repo: `MaestroConTiempo/WebIAMARXAbona2`

## Flux de treball
- **No hi ha servidor local disponible** (npm/Node no estan al PATH de bash)
- Fer canvis → commit → `git push origin main` → Vercel desplega automàticament
- L'usuari verifica els canvis directament a la URL de Vercel, no en preview local

## Estructura
```
app/
  page.jsx     ← tot el contingut i components de la landing
  layout.jsx   ← layout base
```

## Idioma i contingut
- Tot el contingut és en **català**
- Projecte: servei d'implementació d'IA per a escoles ("Centre IA en Marxa")
- Públic: directors i equips pedagògics d'escoles

## Seccions actuals (en ordre)
1. Header (nav fixa)
2. Hero + mètriques animades
3. Problema — "Què passa al vostre centre?"
4. Cost real — "Quin és el cost real de continuar com ara?"
5. Programa — 3 fases (Diagnosi · Implantació · Expansió)
6. Què tindrà el centre — 2 columnes (direcció / claustre) + 4 lliurables
7. Exemples reals — targetes Abans/Després
8. Testimonis
9. 4 passos
10. CTA final + contacte (email + WhatsApp)
11. Footer

## Convencions del codi
- Components d'animació: `FadeItem` (per ítem) i `useInView` (per comptadors)
- Comptadors animats: `useCounter(target, inView, duration)`
- Icones: `lucide-react` (ArrowRight, Users, BookOpen, Globe, ArrowUpRight)
- Colors principals: `blue-900` (bleu fosc), `blue-50` (fons suau)

## Commits
- Sempre en català o anglès, descriure QUÈ i PER QUÈ
- Afegir `Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>`
- Push sempre a `main`
