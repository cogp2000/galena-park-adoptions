# Galena Park Kennel adoption site

Updated deployment package: August 7, 2026.

## Deploy with GitHub + Netlify

1. **Replace the old repository contents with the contents of this ZIP.** In particular, overwrite any existing `netlify.toml`; the included file is valid TOML and intentionally minimal.
2. Commit and push to the `main` branch.
3. In Netlify, connect the repository (or keep the existing connected site).
4. Build command: leave blank. Publish directory: `.` (repository root).
5. Deploy. This is a static HTML/CSS/JavaScript site and needs no npm install or framework build.

## Adoption inquiry form

The form name is `adoption-inquiry` and uses Netlify Forms. After the first successful deploy, confirm that Netlify detects the form, then add an email notification for `humane@cityofgalenapark-tx.gov` in the site's Forms settings.

## Important

- The package contains all 13 kennel dogs from the supplied bio sheets.
- Snowball is marked **Adoption pending**, carrying forward the latest project status.
- Heartworm-positive profiles clearly say to ask about sponsored treatment.
- Availability, health information, temperament, visiting hours, and adoption requirements should still be confirmed by kennel staff.

## Netlify configuration

`netlify.toml` contains only:

```toml
[build]
publish = "."
```

This avoids the configuration parsing issue caused by malformed/unsupported configuration.
