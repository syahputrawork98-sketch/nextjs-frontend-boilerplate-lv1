# Nextjs Frontend Boilerplate Lv1

Boilerplate Next.js (App Router) sederhana untuk tim kecil. Fokus: struktur folder rapi + UI kit atomik dasar.

## Stack
- Next.js (App Router)
- TypeScript
- Tailwind CSS v4

## Struktur Folder
src/
components/
ui/ # komponen atomik
layout/ # layout primitives (Container, Header, Footer)
sections/ # blok halaman
lib/ # helpers, utils
styles/ # global css, theme tokens
app/ # Next.js routes

## Layout
- `Header` → `src/components/layout/header.tsx`
- `Footer` → `src/components/layout/footer.tsx`
- `Container` → `src/components/layout/container.tsx`

## Sections
- `Hero` → `src/components/sections/hero.tsx`
- `Features` → `src/components/sections/features.tsx`
- `Home` page menggabungkan `<Hero />` + `<Features />`



## Getting Started
```bash
npm install
npm run dev
Buka http://localhost:3000.

UI Kit (Atomik)
Contoh komponen dasar:

Button → button.tsx
Input → input.tsx
Contoh pemakaian:

tsx

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";

export default function Example() {
  return (
    <div className="flex gap-2">
      <Input placeholder="Email" />
      <Button>Submit</Button>
    </div>
  );
}


Sections
Hero → hero.tsx
Home page menggunakan <Hero />

Konvensi
ui/ = komponen atomik & reusable
layout/ = struktur layout dasar
sections/ = blok halaman
gunakan alias @/ untuk import dari src/

Next Steps (Opsional)
tambah komponen UI lain (Card, Badge, Modal)
tambah Header dan Footer
setup linting/formatting rule tim