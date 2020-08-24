## Styling

This document is going to cover what you need to know about designing / modifying the pages in doctorlingo.

We use the Ant Design library when we're building out our website components.

You can explore their components here: https://ant.design/components/button/

After helping build what we have so far, I'm seeing a top-down approach.

### Style hierarchy

1.) Try to use ant design features as much as possible before going into custom styling

  - use the row gutters / columns / layout, etc. to make the spacing make sense with their grid system

2.) Try to stick in the ant design theme file

  - `/src/themes/default.js`
  - allows us to not have to add or remove anything in the actual components, then we can switch this out easily if we ever have like "holidaytheme.js" or something.
  - if we can use just items 1 and 2 of the hierarchy, that to me makes the most sense. Because then we just copy default.js from the themes folder, and modify whatever we want to get a new theme, and can "switch" it to be live, or integrate it with user options pretty easily.

3.) Use a .css file, import it into the component, then add a `className={""}`

  - this is sort of the old school way, not using the less theme from ant
  - try to stay away from anything with sizing like #1
  - using CSS flex properties also seems to conflict with antd's implementation of flex

4.) Use a `style={}` as a last resort

  - I have a couple of these still, like the header for a red admin button, the width of the search to be 100%, etc.
  - We should work to get 0 style={} on the site, and use just #1/2


