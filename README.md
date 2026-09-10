# Patfee widget test host

Static, noindex page used only to verify that the Patfee widget works from an
authorized third-party origin. It contains no secret, business data or Patfee
calculation code.

Published reference pages:

- Production: `https://giginventions.github.io/patfee-widget-test/`
- Staging: `https://giginventions.github.io/patfee-widget-test/staging/`

The production page loads `https://patfee.org/widget/v1.js`. Its widget registry
must authorize the exact parent origin `https://giginventions.github.io`.

The staging page includes the dedicated audit widget by default. Both pages
reserve 720 pixels before loading the widget script so Lighthouse measures the
integration without an artificial layout shift.
