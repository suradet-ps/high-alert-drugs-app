# High Alert Drugs App

```
██╗  ██╗██╗ ██████╗██╗  ██╗ █████╗ ██╗     ███████╗██████╗ ████████╗
██║  ██║██║██╔════╝██║  ██║██╔══██╗██║     ██╔════╝██╔══██╗╚══██╔══╝
███████║██║██║  ███╗███████║███████║██║     █████╗  ██████╔╝   ██║
██║  ██║██║██║   ██║██║  ██║██╔══██║██║     ██╔══╝  ██╔══██╗   ██║
██║  ██║██║╚██████╔╝██║  ██║██║  ██║███████╗███████╗██║  ██║   ██║
╚═╝  ╚═╝╚═╝ ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝╚══════╝╚═╝  ╚═╝   ╚═╝
```

---

## ◆ PULSE

A high-alert drug does not announce its risk on the label; the
pharmacist must already know. This app puts the knowledge at the point
of care: instant search across high-alert medications by generic or
trade name, full monographs - dosage, administration, side effects,
monitoring parameters - and an installable PWA that keeps the answers
offline, in the pocket, in the ward. Optimized for Thai healthcare
settings, from the Prompt typeface to the screens it sits on.

| Search ▣ | Monographs ▣ | Offline PWA ▣ | Thai-first ▣ |
|---|---|---|---|

*The reference - search, monograph, install - is sealed.*

> Built with Vue 3 + Vite, backed by Supabase, shipped as an
> installable PWA to Firebase Hosting.
>
> **suradet-ps**, artifact keeper

---

## ◆ IGNITION

One runtime, four commands.

```
⟫ git clone https://github.com/suradet-ps/high-alert-drugs-app.git
⟫ cd high-alert-drugs-app
⟫ npm install
⟫ npm run dev
```

Open [http://localhost:5173](http://localhost:5173).

<details>
<summary>Environment</summary>

A `.env` file with the Supabase credentials:

```
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

</details>

---

## ◆ ANATOMY

One search box, one monograph, a reference that never needs a signal.

- **Searches** - instant lookup by generic or trade name - the drug
  answers as the letters land, no submit, no waiting.
- **Explains** - each monograph carries dosage, administration, side
  effects, and monitoring parameters - the four questions a
  pharmacist asks before any high-alert order.
- **Installs** - a `vite-plugin-pwa` service worker makes the app
  installable and offline-capable: the ward's wifi dies and the
  reference does not.
- **Renders** - Vue 3 reactivity with custom CSS variables theming,
  and the Prompt font family tuned for Thai text - the page reads
  like the setting it serves.
- **Serves** - Supabase holds the monograph data; the client fetches
  and caches; Firebase Hosting ships the build.

---

## ◆ RITUALS

**The core ceremony** - the point-of-care lookup:

1. Open the app - installed on the phone, ready in the ward.
2. Type the drug's name, generic or trade. The list answers as you
   type.
3. Open the monograph: dosage, administration, side effects,
   monitoring - the four questions answered on one screen.
4. Close it. The knowledge stays in the pocket, and in the cache.

**The ceremony of the offline ward** - the network drops mid-shift
and the reference does not flinch: the monographs were cached when
the phone was online, so the care never waits on a spinner.

**The ceremony of the Thai page** - the interface is built for the
setting it serves: Thai healthcare, Thai typeface, and answers that
read in the language the ward speaks.

---

## ◆ ECHOES

**Where this artifact is heading**

```
search    ▸ generic + trade name instant lookup ─────────────────────── ▸ sealed
monograph ▸ dosage, administration, side effects, monitoring ────────── ▸ sealed
offline   ▸ installable PWA, cached reference ───────────────────────── ▸ sealed
localize  ▸ Prompt typography for Thai settings ─────────────────────── ▸ sealed
```

**Raising the artifact** - the Supabase client lives in `src/lib/`;
the components in `src/components/`. Open an issue first to discuss
a change.

**Status** - dependencies are maintained through Renovate; releases
deploy to Firebase Hosting.

---

```
  ─────────────────────────────────────────
   A high-alert drug forgiven once
   is a high-alert drug remembered forever.
  ─────────────────────────────────────────
```

Licensed under the [MIT License](LICENSE).