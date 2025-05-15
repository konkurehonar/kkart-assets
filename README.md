# kkart-assets

A comprehensive repository of graphic assets for the Koushk Konkur-Honar educational platform. This repository serves as a central hub for all SVG icons, logos, illustrations, and UI elements used across our web applications and educational materials.

## Repository Structure

- `/icons` - General purpose icons used throughout the platform
- `/logos` - Brand logos and identity elements
- `/illustrations` - Educational and decorative illustrations
- `/ui-elements` - User interface components and design elements

## Features

- **Automated SVG Optimization** - All SVG files are automatically optimized when added to the repository
- **Accessibility Enhanced** - SVGs include proper ARIA attributes and bilingual metadata
- **Theme Compatibility** - Colors converted to currentColor for seamless theme integration
- **Consistent Naming** - Standardized naming conventions for easy asset discovery
- **Bilingual Support** - All assets include both Farsi and English metadata

## Optimization Process

When you add an SVG file to this repository, our automated workflow:

1. Cleans and minifies the SVG code
2. Removes fixed dimensions for better scalability
3. Converts fill colors to currentColor for theme compatibility
4. Adds accessibility attributes (role="img", aria-label)
5. Generates bilingual title and description tags
6. Creates tags based on the filename
7. Produces an optimized version with the `.optimized.svg` extension

## Usage

### Direct CDN Usage

```html
<img src="https://cdn.jsdelivr.net/gh/username/KKArt-assets@main/icons/icon-name.optimized.svg" alt="Icon description" />
```

### As a Git Submodule

```bash
git submodule add https://github.com/username/KKArt-assets.git assets/graphics
```

### In React Components

```jsx
import { ReactComponent as IconName } from 'path/to/icon-name.optimized.svg';

function MyComponent() {
  return <IconName className="icon" />;
}
```

## Contributing

1. Place SVG files in the appropriate directory
2. Use descriptive filenames with hyphens (e.g., `user-profile.svg`, `login-button.svg`)
3. Commit and push your changes
4. The GitHub Action will automatically create optimized versions

## License

All assets in this repository are proprietary and belong to Koushk Konkur-Honar educational platform. Unauthorized use, distribution, or modification is prohibited.
