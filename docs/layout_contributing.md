### Template
Start with `templates/layout.json`.

---

### Layout ID
Use the layout name as the **ID** in **snake_case**  
(e.g., `"Simple Card"` → `simple_card`).
Must be unique.

---

### Versioning
Increment the `version` number whenever an existing layout is modified or improved (e.g., `1.0 → 1.1`) [`major.minor`].

---

### Preview
- **Direct link** ending with `.png`, `.jpg`, `.gif`, `.mp4`, etc
- Use trusted platforms like Postimg, Imgur, GitHub user content, or place inside the repo’s `images/` folder.  
- Keep file size minimum.  
- **1:1 aspect ratio** for image previews with the widget centered.  
- **File name format:**  
  `layout_id-theme_id.extension`
   
  > Example: `simple_card-sunset_glow.jpg`

---

### Structure Object
- The `structure` field defines the **actual widget layout**.  
- Use `tasker variables` for dynamic properties (e.g., `%text_size_event_days`, `%max_lines_event_title`, etc).
- Following variables (as many required) should be used for best compatibility with themes.

```json
%font_primary
%font_secondary
%image
%icon
%corner_radius
%color_accent
%color_divider
%color_outline
%color_highlight
%background_color
%background_color_icon
%background_color_event_title
%background_color_event_date
%background_color_event_alert
%background_color_event_days
%background_color_event_label
%text_color_event_title
%text_color_event_date
%text_color_event_alert
%text_color_event_days
%text_color_event_label
%command (REQUIRED)
```

---

### Command
Must include `%command` variable for command & `DT` for command prefix.

This is required for widget interaction.

---

### Defaults Object
Must include all variables used in structure in defaults. Overrides theme variables.

e.g.,
```json
"defaults": {
    "text_size_event_title": "22",
    "text_size_event_days": "75",
    "max_lines_event_title": "2"
}
```
---

### Validation 
  - Check JSON via [jsonlint.com](https://jsonlint.com).  
  - Ensure unique IDs and all required fields are present.
  - The JSON is properly formatted (use indentation).
  - Preview link works and image/video loads correctly.

### Tips
- Set `Use Material You Colors` to `true` for texts.
