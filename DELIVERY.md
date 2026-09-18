# Project delivery checklist

Use this as the standard for Odoo work under Uss Alilm / sirelkhatimgamal.

## Repository

- [ ] Repository lives in the **sirelkhatimgamal** organization for production clients
- [ ] Name is lowercase, hyphenated, and describes the client or product (`client-odoo-addons`)
- [ ] Description and topics are set (`odoo`, `odoo18`, `python`, `ksa`)
- [ ] README explains purpose, Odoo version, and module list
- [ ] `.gitignore` excludes `__pycache__`, `.pyc`, data dumps, `.zip`, and secrets
- [ ] Default branch is `main` (or `18.0` for versioned Odoo repos)

## Modules

- [ ] Each addon has `__manifest__.py`, `__init__.py`, security, views, and README
- [ ] Technical names are unique and stable
- [ ] No `++folder++` or `folder+++` experiment copies in production branches
- [ ] Third-party zips are unpacked or tracked as Git submodules, not committed as binaries
- [ ] Odoo Enterprise code is never published publicly

## Quality

- [ ] Access rights and record rules are explicit
- [ ] Reports print correctly in Arabic and English where required
- [ ] Cron jobs and mail templates are documented
- [ ] Upgrade notes exist when a module depends on a specific Odoo minor version

## Go-live

- [ ] Staging database tested with a recent production copy (private, never on GitHub)
- [ ] Users trained on the changed screens
- [ ] Backup and Cloudpepper/deployment notes recorded
