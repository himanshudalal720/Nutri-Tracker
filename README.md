# NextLevelFit

NextLevelFit is a modern health and fitness website built with React.js and Sass. It promotes a healthy lifestyle by offering features like calorie calculation, recipes, and meal planning.

---

## Features

- **Responsive Design:** Optimized for mobile, tablet, and desktop devices.
- **Recipes Search:** Find recipes based on ingredients or popular healthy foods.
- **Calorie Calculator:** Track your daily calorie needs using the Fitness Calculator API.
- **Favorites Management:** Save and manage favorite recipes using local storage.
- **Contact Form:** Easily get in touch via an integrated contact form.

---

## Docs

### Fonts
- **Source:** [Google Fonts](https://fonts.google.com/)
- **Fonts Used:**
  - Courgette
  - Raleway
  - Poppins

### Icons
- **Source:** [Font Awesome](https://fontawesome.com/)

---

### Images

#### **Home Background**
- **Source:** [Pexels - Alleksana](https://www.pexels.com/photo/fresh-papaya-slices-on-white-ceramic-plate-4113866/)

#### **Services Background**
- **Source:** [Pexels - Ella Olsson](https://www.pexels.com/photo/fruit-salads-in-plate-1640774/)

#### **Services Icons**
- **Source:** [UnDraw](https://undraw.co/)

#### **Recommendation Section**
- **Pexels - Antoni Shkraba**:
  - [Packed Food in Containers](https://www.pexels.com/photo/packed-food-in-colorful-containers-5852326/)
  - [Bread with Peanut Butter and Banana](https://www.pexels.com/photo/bread-with-peanut-butter-and-sliced-banana-on-white-ceramic-plate-6823293/)
  - [Sliced Bread with Vegetables and Fruits](https://www.pexels.com/photo/sliced-bread-with-sliced-vegetables-and-fruits-on-white-ceramic-plate-5589027/)
- **Pexels - Roman Odintsov**:
  - [Grilled Vegetables and Fried Egg](https://www.pexels.com/photo/grilled-vegetables-and-fried-egg-with-beans-and-sausage-4552980/)

#### **Recipes Page Background**
- **Source:** [Pexels - Viktoria Slowikowska](https://www.pexels.com/photo/assorted-fresh-vegetables-in-messy-composition-5678044/)

- **Image Compression:** [Image Compressor](https://imagecompressor.io/)

---

## Features Explanation

### Contact Form
- **Service Used:** [FormSubmit](https://formsubmit.co/)
- The form is submitted using a `fetch` POST request to the URL:  
  `https://formsubmit.co/ajax/[admin_email_mask]`
- **Activation Steps:**
  1. Deploy the website.
  2. Submit the form once.
  3. Activate the form using the activation link sent to the admin email.
- Once activated, the admin will receive feedback/messages directly in their inbox.

---

### Recipes Search
- **Service Used:** [Edamam Recipe Search API](https://developer.edamam.com/edamam-recipe-api)
- **Current Plan:** Free Developer Package:
  - **10,000 API calls/month**
  - **10 calls/minute throttling**
- **How It Works:**
  1. User types a query (e.g., a food or ingredient) and clicks the search button.
  2. User clicks one of the top 10 healthy foods listed.
- **API Endpoint:**
  ```plaintext
  https://api.edamam.com/api/recipes/v2?type=public&q=${query}&app_id=${id}&app_key=${key}
