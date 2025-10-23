### Template 
Start with `templates/theme.json`.  

### Theme ID 
Use the theme name as ID but in **snake_case** (e.g., `"Sunset Glow"` → `sunset_glow`).  

### Versioning
Increment the `version` for each update.  

### Preview  
- Use a **direct link** (`.png`, `.jpg`, `.gif`, or `.mp4`).  
- Host on **Postimg**, **Imgur**, **GitHub user content** or add to `images/` folder of this repo.  
 - Keep files ≤ **1 MB**.
 - Crop preview to 1:1 if image   
 - File name format: `theme_id-layout_id.extension`  

### Style Object
  - All fields are **required**.  
  - Text colors use `#RRGGBB`; others may use `#AARRGGBB`.  

### Validation 
  - Check JSON via [jsonlint.com](https://jsonlint.com).  
  - Ensure unique IDs and all required fields are present.
