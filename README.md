# **Pokémon Search App**  

A React-based web application that allows users to search for Pokémon, view their images, and load more Pokémon dynamically using the **PokeAPI**.  

## **Live Demo**  
🔗 [[Live Link](https://pokemon-search-anyone.netlify.app/)]
## **Tech Stack**  
- **Frontend:** React.js, JavaScript, CSS  
- **API:** [PokeAPI](https://pokeapi.co/api/v2/pokemon)  

## **Features**  

### 🚀 **1. Fetch Pokémon Data from PokeAPI**  
- Retrieves a list of Pokémon from **PokeAPI** and displays their **ID, name, and sprite image**.  
- Uses **async/await** and `Promise.all()` for efficient API calls.  

### 🔄 **2. Infinite Scrolling & Load More Functionality**  
- Loads Pokémon **in batches of 50** to improve performance.  
- Clicking **"Load More"** fetches the next set of Pokémon dynamically.  

### 🔍 **3. Search Functionality**  
- Users can **search for Pokémon by name**.  
- The search **filters Pokémon dynamically** without requiring additional API calls.  

### ⚡ **4. Optimized State Management with React Hooks**  
- **`useState`** manages Pokémon data, loading state, and search input.  
- **`useEffect`** fetches Pokémon data on component mount and when `offset` updates.  

### 🛠 **5. Error Handling & Loading States**  
- Displays a **loading indicator (`Loading...`)** when fetching data.  
- Handles API failures and shows a **user-friendly error message**.  
- Ensures missing Pokémon images **do not break the app**.  

### 🖼 **6. Safe Data Handling & Fallbacks**  
- Uses **optional chaining (`?.`)** to prevent crashes due to missing data.  
- Provides **fallback images** for Pokémon that do not have official artwork.  
- Includes an **`onError` handler** in the `<img>` tag to replace broken images.  

### 📂 **7. Modular Component Structure**  
- **`Pokemon.jsx`** → Fetches data, manages state, handles search and pagination.  
- **`PokemonCard.jsx`** → Displays individual Pokémon details (name & image).  
- **`index.css`** → Contains styling for a clean and responsive UI.  

## **Installation & Setup**  

1. **Clone the repository**  
   ```sh
   git clone https://github.com/yourusername/pokemon-search-app.git
   cd pokemon-search-app
