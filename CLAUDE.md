# Guidelines for DSI Course Repository

## Repository Structure
- `documentos/`: Core course documentation
- `evaluaciones/`: Assessment materials (exams and challenges)
- `temario/`: Course syllabus and lecture materials
- `images/`: Images and diagrams used throughout the course

## Content Guidelines
- Use Markdown for all documentation
- When creating PlantUML diagrams, place source files in `temario/modelosUML/`
- Rendered diagram images should go in `images/modelosUML/`
- Reference images using relative paths
- Maintain consistent heading hierarchy (# for title, ## for sections)
- Use lists for sequential instructions or related items
- Include links to related materials when appropriate

## Naming Conventions
- Files: kebab-case (e.g., `modelo-negocio.md`)
- Folders: camelCase where appropriate
- Image files: descriptive names that reflect content

## Working with this Repository
- Commit messages should clearly describe changes
- Always pull latest changes before editing content
- Keep image sizes reasonable (compress if necessary)