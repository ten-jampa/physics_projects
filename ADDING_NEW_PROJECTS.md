# Adding New Projects to Physics Projects Portfolio

This guide explains how to add new physics projects to your portfolio website.

## 📋 Prerequisites

Before adding a new project, ensure you have:
- Your project files (notebooks, data, results, etc.)
- Project description and methodology
- Key results and findings
- Technologies and tools used

## 🚀 Step-by-Step Process

### 1. Create Project Directory

Create a new directory for your project in the root folder:

```bash
mkdir "Your Project Name"
```

**Note**: Use descriptive names that clearly indicate the project focus.

### 2. Add Project Files

Copy your project files into the new directory:

```
Your Project Name/
├── project-notebook.ipynb
├── data/
├── results/
├── README.md (optional)
└── other-files/
```

### 3. Create Project Web Page

Copy the template file and customize it:

```bash
cp templates/new-project-template.html projects/your-project-name.html
```

### 4. Customize the Project Page

Edit the new HTML file and replace the placeholder content:

#### Required Changes:
- `[PROJECT_NAME]` → Your actual project name
- `[PROJECT_DESCRIPTION]` → Brief project description
- `[ICON_CLASS]` → FontAwesome icon class (e.g., `fas fa-microscope`)
- `[DETAILED_PROJECT_DESCRIPTION]` → Comprehensive project overview

#### Feature Section:
- `[FEATURE_TITLE_1]` → First key feature
- `[FEATURE_DESCRIPTION_1]` → Description of first feature
- `[FEATURE_ICON_1]` → Icon for first feature
- Repeat for features 2 and 3

#### Methodology Section:
- `[STEP_TITLE_1]` → First methodology step
- `[STEP_DESCRIPTION_1]` → Description of first step
- Repeat for all methodology steps

#### Results Section:
- `[RESULT_TITLE_1]` → First key result
- `[RESULT_DESCRIPTION_1]` → Description of first result
- Repeat for all results

#### Technologies Section:
- `[TECH_NAME_1]` → First technology/tool
- `[TECH_DESCRIPTION_1]` → Description of first technology
- `[TECH_ICON_1]` → Icon for first technology
- Repeat for all technologies

### 5. Update Main Index Page

Edit `index.html` to add your new project to the projects section:

```html
<!-- Add this inside the projects row -->
<div class="col-lg-6">
    <div class="card project-card">
        <div class="card-img-top d-flex align-items-center justify-content-center">
            <i class="[YOUR_ICON_CLASS] text-white" style="font-size: 4rem;"></i>
        </div>
        <div class="card-body">
            <h5 class="card-title">[YOUR_PROJECT_NAME]</h5>
            <p class="card-text">
                [YOUR_PROJECT_DESCRIPTION]
            </p>
            <div class="mb-3">
                <span class="badge bg-primary me-2">[TAG_1]</span>
                <span class="badge bg-secondary me-2">[TAG_2]</span>
                <span class="badge bg-info me-2">[TAG_3]</span>
                <span class="badge bg-success">[TAG_4]</span>
            </div>
            <a href="projects/[YOUR_PROJECT_FILE].html" class="btn btn-primary">
                <i class="fas fa-external-link-alt me-2"></i>View Project
            </a>
        </div>
    </div>
</div>
```

### 6. Update Navigation

Add your project to the navigation menu in all project pages:

```html
<li class="nav-item">
    <a class="nav-link" href="your-project-name.html">[YOUR_PROJECT_NAME]</a>
</li>
```

### 7. Update README.md

Add your project to the README file:

```markdown
### 3. [YOUR_PROJECT_NAME]
- **Focus**: [PROJECT_FOCUS]
- **Technologies**: [TECHNOLOGIES_USED]
- **Key Features**:
  - [FEATURE_1]
  - [FEATURE_2]
  - [FEATURE_3]
- **Files**: `[PROJECT_DIRECTORY]/[FILES]`
```

## 🎨 Customization Tips

### Icons
Use FontAwesome icons for consistency:
- Physics: `fas fa-atom`, `fas fa-wave-square`, `fas fa-microscope`
- Data: `fas fa-chart-line`, `fas fa-database`, `fas fa-calculator`
- Tools: `fab fa-python`, `fas fa-code`, `fas fa-cogs`

### Colors
The site uses a consistent color scheme:
- Primary: `#2c3e50` (Dark Blue)
- Secondary: `#3498db` (Blue)
- Accent: `#e74c3c` (Red)
- Light Background: `#ecf0f1` (Light Gray)

### Styling
- Keep descriptions concise but informative
- Use consistent formatting across all projects
- Include relevant badges and tags
- Ensure responsive design works on mobile

## 📁 File Structure Example

After adding a new project, your structure should look like:

```
physics_projects/
├── index.html
├── projects/
│   ├── gravitational-waves.html
│   ├── weak-mixing-angle.html
│   └── your-new-project.html
├── Your New Project/
│   ├── project-notebook.ipynb
│   ├── data/
│   └── results/
├── templates/
│   └── new-project-template.html
└── README.md
```

## 🔧 Testing

After adding a new project:

1. **Test locally**: Open the HTML files in a browser
2. **Check navigation**: Ensure all links work correctly
3. **Verify responsive design**: Test on different screen sizes
4. **Review content**: Check for typos and formatting issues

## 🚀 Deployment

Once you've added your new project:

1. Commit your changes:
   ```bash
   git add .
   git commit -m "Add new project: [PROJECT_NAME]"
   git push origin main
   ```

2. GitHub Pages will automatically rebuild your site
3. Your new project will be live at: `https://[username].github.io/physics_projects/`

## 📝 Best Practices

- **Consistency**: Follow the same format as existing projects
- **Clarity**: Write clear, concise descriptions
- **Completeness**: Include all relevant information
- **Visual Appeal**: Use appropriate icons and styling
- **Accessibility**: Ensure good contrast and readable fonts

## 🆘 Troubleshooting

### Common Issues:
- **Broken links**: Double-check all file paths
- **Styling issues**: Ensure CSS classes are consistent
- **Navigation problems**: Verify all navigation links are updated
- **Mobile responsiveness**: Test on different devices

### Getting Help:
- Check existing project pages for examples
- Review the template file for guidance
- Ensure all required files are in the correct locations

---

**Happy coding!** 🚀

This guide should help you seamlessly add new projects to your physics portfolio. Remember to maintain consistency and quality across all projects. 