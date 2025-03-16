## Technologies Used
- **HTML5** - Structuring the content.
- **CSS3** - Styling and layout (Flexbox & Grid).
- **Phosphor Icons** - Icon library for social media links.

## Layout Approach
The website uses a combination of **Flexbox** and **CSS Grid** for efficient layout and responsiveness.

### **1. Flexbox Usage**
- **Navigation Menu (`.navmenu`)**
  ```css
  .navmenu {
    display: flex;
    gap: 1.5rem;
  }
- **Social Media Buttons (`.child-container`)**
  ```css
    .child-container {
    display: flex;
    gap: 1rem;
    align-items: center;
  }
- **Header (`header`)**
  ```css
  header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

### **2. CSS Grid Usage**
- **Homepage Layout  (`.home`)**
  ```css
  .home {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  gap: 1rem;
}

## Responsive Design
- **For Tablets (`max-width: 768px`)**
  ```css
  @media (max-width: 768px) {
  .home {
    grid-template-columns: 1fr; /* Switch to single-column */
    text-align: center;
  }
  .home-img {
    order: -1; /* Move image above text */
  }
  .child-container {
    justify-content: center; /* Center-align buttons */
  }
  .navmenu {
    flex-direction: column;
    text-align: center;
  }
}

- **For Mobile  (`max-width: 480px`)**
  ```css
  @media (max-width: 480px) {
  .home-text h2 {
    font-size: 2rem;
  }
  .btn {
    font-size: 10px;
    padding: 0.75rem;
  }
  .child-container {
    flex-direction: column;
    gap: 0.5rem;
  }
  .scroll-btn {
    font-size: 0.8rem;
  }




  
