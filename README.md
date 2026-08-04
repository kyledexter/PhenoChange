# PhenoChange website

This repository contains the GitHub Pages website for **PhenoChange: A network for monitoring the phenology of tropical dry forests and savannas**.

## Publish on GitHub Pages

1. Create a public GitHub repository named `PhenoChange` under the account `kyledexter`.
2. Upload all files and folders from this package to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. After deployment, the site should appear at `https://kyledexter.github.io/PhenoChange/`.

## Editing content

- Main page text: edit the corresponding `.md` file in the repository root.
- People: edit `_data/people.yml`.
- Institutions: edit `_data/institutions.yml`.
- Publications: edit `_data/publications.yml`.
- Navigation: edit `_data/navigation.yml`.
- Colours and layout: edit `assets/css/style.css`.
- Funding text in the footer: edit `_includes/footer.html`.

## Adding images

Create folders such as:

- `assets/images/people/`
- `assets/images/institutions/`
- `assets/images/sites/`
- `assets/images/funders/`

Use lowercase filenames without spaces, for example `kyle-dexter.jpg`. In YAML, paths begin with `/assets/images/...`.

## Previewing locally

With Ruby and Bundler installed:

```bash
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000/PhenoChange/`.

## Notes

The website uses the GitHub Pages-supported Jekyll system. The current visual mark is a temporary leaf-and-sun device and can be replaced once a formal PhenoChange logo is developed.
