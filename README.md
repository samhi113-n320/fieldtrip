## Field Trip Project

### Project Summary

This website consists of a gallery of Native American jewelry and a tool to design your own using the same techniques. 

### Core Webpages

- Home
  - Introduces site to user, begins with hero content and information about gallery and items as a whole
- Gallery
  - Styled to reflect items as showcased in real-life gallery. Will include sliding magnifying glass.
- Gallery Item (slug)
  - Each item will dynamically load the slug site with descripted content.
- Design It
  - The fun part of the site! The designer tool will allow users to create pieces of jewelry and then will be rated by AI, with critique and guidance for future designs given.

### Design Choices

#### List any websites that you might reference to influence your styling choices. List any colors used and what they were used for. 
https://eiteljorg.org/ - I mean, why wouldn't I? The home of these pieces should be well-represented in the design of the site. The Eiteljorg's yellow and orange colors would be heavily utilized.
Would also use the in-person gallery as guidance, likely making the site dark, which helps emphasize the bright, vibrant colors of the pieces.

#### Describe your data structure with rationale.
- Tables:
  - item
  - gallery
  - galleryItem (to break down M:M table)
- Connections:
  - Business Sense: Each item can belong in many galleries, depending on if it fits multiple themes/stories.
  - item -> galleryItem  -  one : many  -  This allows one item's information to be inserted into multiple galleries.
  - gallery -> galleryItem  -  one : many - This allows one gallery to house multiple items.
