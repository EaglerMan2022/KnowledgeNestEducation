# KnowledgeNestEDU

An account-free, school-style learning dashboard with math practice, a calculator, a class schedule, homework tracking, and locally saved progress.

## Run locally

Open `index.html` in a modern browser, or serve this directory with any static web server. The GBA player loads from its emulator CDN. The 3DS option opens the separate Azahar Web project, which needs a browser supporting WebAssembly threads and cross-origin isolation.

## Features

- Arithmetic practice with a saved count of correctly answered questions.
- Student dashboard with attendance, a sample class schedule, subjects, and a homework checklist.
- Progress and planner checkboxes saved in local browser storage; no account or sign-in required.
- After 50 correct answers, or the calculator unlock, choose the GBA player or open the separate 3DS browser emulator.

## Emulator notes

The GBA option runs within this site. The 3DS option opens [Azahar Web](https://github.com/Shubin123/azahar_web) in a separate tab because its WASM threads require cross-origin isolation, and this school site cannot grant that isolation to a cross-origin embedded frame. Azahar Web's README documents IndexedDB-backed save states on that site's origin; it also notes that normal in-game save files are not persisted by its web build yet. Save states remain browser-managed and are not guaranteed against browser data deletion or storage eviction.

The 3DS web port is experimental. It expects a decrypted game dump and its actual compatibility and speed depend on device/browser. No commercial game files are bundled. Use only game files you have the right to use.
