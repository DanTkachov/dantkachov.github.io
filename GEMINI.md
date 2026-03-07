# Role
Act as an Expert Creative Frontend Developer specializing in SVG manipulation and Anime.js.

# Task
Build a lightweight, single-file (HTML/CSS/JS) frontend component for a mock interviewer application. The UI should feature a stylized "neural network topology" that visually forms a wireframe landscape (scenic grasslands in the foreground, mountains in the background).

# Visual Architecture & Tech Stack
- **Tech Stack:** HTML5, CSS3, inline SVG, and Anime.js (loaded via CDN). NO Three.js or WebGL.
- **The Grid/Nodes:** Generate a set of SVG `<circle>` elements representing "neurons" and `<line>` or `<path>` elements connecting them.
- **The Landscape Shape:** Position the nodes using 2D coordinates to create a forced-perspective landscape. The bottom nodes should be denser and flatter (grasslands), while the top/background nodes should peak into jagged triangles (mountains).
- **Aesthetic:** Dark mode, cyber-organic, or "vapor clinic" style. The nodes should glow slightly, and the connecting lines should have low opacity.

# Animation Requirements (via Anime.js)
1. **The Breathe Effect:** Every single node (neuron) should float continuously up and down along the Y-axis.
2. **Staggered Timing:** The floating animation must be staggered or randomized using Anime.js's `stagger` or random duration functions so the landscape looks like it is organically breathing, rather than moving in one rigid block.
3. **Line Tracking:** The SVG lines connecting the nodes must stay attached to the nodes as they float. (Hint: animate the `cy` attributes of the circles, and the `y1`/`y2` attributes of the corresponding lines simultaneously, or wrap node-groups in `<g>` tags and animate the groups).

# Output Generation
Provide the complete, workable code in a single HTML block. Do not use external CSS or JS files other than the Anime.js CDN link. Ensure the code is heavily commented so I can adjust the landscape coordinates and animation timing later.