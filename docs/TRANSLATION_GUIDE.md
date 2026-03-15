# Translation Guide / Guide de Traduction

## How to Contribute a Translation / Comment contribuer une traduction

### Step 1: Choose Your Language / Choisissez votre langue

Check [TRANSLATIONS.md](../TRANSLATIONS.md) to see if your language is already started.

### Step 2: Create Translation File / Créez le fichier de traduction

1. Copy the English file (e.g., `README.md`)
2. Rename it with language code (e.g., `README.fr.md` for French)
3. Translate the content, keeping the structure intact

**File naming convention:**
- `README.md` → `README.[lang].md`
- Examples: `README.fr.md`, `README.de.md`, `README.es.md`, `README.it.md`

### Step 3: Translate Content / Traduisez le contenu

**Important rules:**
- ✅ Keep all Markdown formatting (headers, lists, links)
- ✅ Preserve image links and external URLs
- ✅ Maintain the same structure and section order
- ✅ Translate naturally, not word-for-word
- ❌ Don't change file paths or links
- ❌ Don't remove images or code blocks

**Example:**
```markdown
<!-- English original -->
## 🎨 UI Customization & Themes
Enhance the visual appeal of Trinity :-)

### [Windows 10 Window Decoration](https://github.com/example)
A specialized window decoration...

<!-- French translation -->
## 🎨 Personnalisation UI & Thèmes
Améliorez l'attrait visuel de Trinity :-)

### [Windows 10 Window Decoration](https://github.com/example)
Une décoration de fenêtre spécialisée...
```

### Step 4: Test Your Translation / Testez votre traduction

1. Open the file in a Markdown viewer
2. Check that all links work
3. Verify images display correctly
4. Read aloud to catch awkward phrasing

### Step 5: Submit / Soumettez

**Option A: Pull Request (Recommended)**
```bash
# Fork the repository
git clone https://github.com/YOUR-USERNAME/seb-q4os-tde-collection.git
cd seb-q4os-tde-collection

# Create branch
git checkout -b translation-[language]-readme

# Add your translated file
cp README.md README.xx.md
# Edit README.xx.md with your translation

# Commit
git add README.xx.md
git commit -m "translate: Add [Language] version of README"

# Push and create PR
git push origin translation-[language]-readme
```

**Option B: GitHub Issue**
1. Create a new issue
2. Title: "Translation: [Language] README"
3. Attach your translated file or paste the content
4. Maintainers will add it to the repository

---

## Translation Standards / Normes de traduction

### Terminology / Terminologie

Keep these terms consistent across translations:

| English | FR | DE | ES |
|---------|----|----|----|
| Trinity Desktop Environment | Environnement de Bureau Trinity | Trinity Desktop Environment | Entorno de Escritorio Trinity |
| Q4OS | Q4OS | Q4OS | Q4OS |
| TDE | TDE | TDE | TDE |
| Kicker panel | panneau Kicker | Kicker-Panel | panel Kicker |
| Start menu | menu Démarrer | Startmenü | menú Inicio |
| Color scheme | schéma de couleurs | Farbschema | esquema de color |
| Window decoration | décoration de fenêtre | Fensterdekoration | decoración de ventanas |

### Style Guidelines / Directives de style

1. **Tone**: Friendly and helpful / Ton amical et utile
2. **Formality**: Use informal "you" (tu/vous selon langue) / Utiliser le tutoiement ou vouvoiement selon la langue
3. **Emojis**: Keep all emojis from the original / Garder tous les emojis
4. **Humor**: Adapt cultural references / Adapter les références culturelles

---

## Updating Existing Translations / Mise à jour des traductions

When the English original changes:

1. Check what changed using git diff or comparison tools
2. Update your translation accordingly
3. Mark as updated in [TRANSLATIONS.md](../TRANSLATIONS.md)

**Quick update process:**
```bash
# Compare your translation with original
diff README.md README.fr.md

# Identify sections that need updating
# Make changes
# Test
# Submit PR
```

---

## Quality Checklist / Liste de contrôle qualité

Before submitting, verify:

- [ ] All text is translated (except proper nouns and technical terms)
- [ ] No typos or grammar errors
- [ ] Links still work
- [ ] Images display correctly
- [ ] Code blocks are unchanged
- [ ] Formatting is preserved
- [ ] Tone matches the original
- [ ] Technical terms are accurate
- [ ] Cultural adaptations make sense

---

## Need Help? / Besoin d'aide?

- **Questions?** Open an issue on GitHub
- **Unsure about a term?** Check other translations in the repo
- **Want to coordinate?** Volunteer as language coordinator in TRANSLATIONS.md

---

## Tools / Outils

**Helpful tools for translators:**

- **Grammarly**: Grammar checking (multiple languages)
- **DeepL**: High-quality machine translation (for reference)
- **Markdown editors**: Typora, VS Code with Markdown preview
- **Git tools**: GitHub Desktop, GitKraken for version control

---

## Thank You! / Merci! / ¡Gracias! / Danke!

Your translations help make Q4OS and TDE accessible to more people worldwide! 🌍

Every contribution counts, from translating a single paragraph to complete documents.

**Happy translating!** 🚀
