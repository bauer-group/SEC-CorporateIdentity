# CSS Variablen

Vollständiges CSS Custom Properties Set für die Implementierung des BAUER GROUP Designsystems.

## Komplettes Token Set

```css
:root {
  /* ─── Primary: Orange ─── */
  --orange-50: #FFF7ED;
  --orange-100: #FFEDD5;
  --orange-200: #FED7AA;
  --orange-300: #FDBA74;
  --orange-400: #FB923C;
  --orange-500: #FF8500;  /* Brand Primary */
  --orange-600: #EA6D00;
  --orange-700: #C2570A;  /* Text AA */
  --orange-800: #9A4509;  /* Text AAA */
  --orange-900: #7C3A0A;

  /* ─── Warm Gray (Unterstützende Farben) ─── */
  --warm-50: #F9F8F6;
  --warm-100: #F0EDEA;
  --warm-200: #E0DBD6;
  --warm-300: #C4BDB7;
  --warm-400: #A69E97;
  --warm-500: #887F78;
  --warm-600: #6B635C;   /* Body Text AA */
  --warm-700: #524B45;   /* Strong Text AAA */
  --warm-800: #3A3430;   /* Headlines, Brand Dark */
  --warm-900: #231F1C;   /* Brand Black */

  /* ─── Brand Neutrals ─── */
  --brand-white: #FFFFFF;
  --brand-light: #F9F8F6;  /* = Warm 50 */
  --brand-dark: #3A3430;    /* = Warm 800 */
  --brand-black: #231F1C;   /* = Warm 900 */

  /* ─── Semantisch ─── */
  --success-100: #DCFCE7;  --success-500: #22C55E;  --success-700: #15803D;
  --warning-100: #FEF9C3;  --warning-500: #EAB308;  --warning-700: #A16207;
  --error-100: #FEE2E2;    --error-500: #EF4444;    --error-700: #B91C1C;
  --info-100: #DBEAFE;     --info-500: #3B82F6;     --info-700: #1D4ED8;

  /* ─── Akzent ─── */
  --accent-blue: #2563EB;
  --accent-teal: #0D9488;
  --accent-amber: #D97706;
  --accent-indigo: #6366F1;

  /* ─── Semantische Aliase ─── */
  --text-primary: var(--warm-900);
  --text-secondary: var(--warm-600);
  --text-muted: var(--warm-500);
  --text-disabled: var(--warm-400);

  --bg-primary: #FFFFFF;
  --bg-subtle: var(--warm-50);
  --bg-muted: var(--warm-100);

  --border: var(--warm-200);
  --border-strong: var(--warm-300);

  /* ─── Typography ─── */
  --font-body: system-ui, -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  --font-mono: ui-monospace, "SF Mono", "Cascadia Code",
    "Segoe UI Mono", Consolas, monospace;
}
```

## Verwendung

```css
body {
  font-family: var(--font-body);
  color: var(--text-primary);
  background: var(--bg-primary);
}

h1, h2, h3 {
  color: var(--warm-800);
}

a {
  color: var(--orange-700);  /* AA-konform */
}

.btn-primary {
  background: var(--orange-500);
  color: white;
}
```
