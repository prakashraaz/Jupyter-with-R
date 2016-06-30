# Using Jupyter notebooks with R in the classroom

<img alt="Jupyter Logo" src="https://avatars1.githubusercontent.com/u/7388996?v=3&s=200"/>
<img alt="R Logo" src="https://www.r-project.org/logo/Rlogo.png"  style="width:200px"/>


# To build your own slides from a Jupyter notebook:

- Ensure the 'Slide' option in the Cell Toolbar is available by selecting
  View → 'Cell toolbar' → 'Slideshow' in the box on the top right of the notebook.
- Identify cells you wish to have rendered as slides by selecting 'Slide type:' as
  'Slide' at the top right of each cell.
  - 'Sub-Slide' is the same as 'Slide' but the animation of slide motion is
    to wipe up (instead of left) off the page.
  - 'Fragment' will append the content of the new cell to the bottom of the existing
    cell on the page.
- Execute this command in a terminal shell:

```shell
export PREFIX=https://cdn.jsdelivr.net/reveal.js/3.0.0; \
   jupyter nbconvert --to slides <your-notebook-name-here>.ipynb \
   --reveal-prefix ${PREFIX}
```
