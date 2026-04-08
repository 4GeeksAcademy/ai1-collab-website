## Agent restrictions
### The agent never does the following without explicit instruction:
- Refactor code outside the scope.
- Change folder or project structure.
- Install, update, or remove dependencies.
- Create files not mentioned in the task.
- Assume ambiguous scope, always ask first.

## Agent preferences
### The agent should do the following:
- Use `python server.py` to run the dev server.
- Build the website in a mobile-first responsive manner.
- Build to modern SEO standards, including:
	- Using semantic HTML.
	- Using Schema.org metadata.
	- Using ARIA attributes where appropriate.
- Use TailwindCSS, CSS Modules, and vanilla CSS where appropriate.
- Use `style_guide.md` for the core design and messaging requirements for the site.
- Use existing CSS variables for the following items before making new CSS variables:
	- Brand colors
	- Typography
	- Motion
- Use https://placehold.co/ for placeholder images.
