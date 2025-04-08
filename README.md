Interactive React Tours Project


An interactive web application built with React that fetches and displays tour package information from an API. Users can browse tours, read descriptions, and remove tours they are not interested in.

**[Live Demo](https://toursprojectnoto.netlify.app/)**


![Screenshot 1](https://github.com/user-attachments/assets/0074a19b-8dbc-4cd9-bce7-a4e305045f8d)
![Screenshot 2](https://github.com/user-attachments/assets/0a87294e-e32e-4d57-ba1b-ea49c9902a7f) 
![Screenshot 3](https://github.com/user-attachments/assets/a30dc942-04e0-4f7c-b2d5-77b3bdaa46a9)




## Features

* **Fetches Tour Data:** Asynchronously fetches tour information from the `course-api.com` endpoint on load.
* **Displays Tours:** Renders fetched tours in a responsive card grid layout.
* **Loading State:** Shows a loading indicator while data is being fetched.
* **Read More/Show Less:** Allows users to expand or collapse longer tour descriptions.
* **Remove Tour:** Users can remove individual tours from the list by clicking the "Not Interested" button.
* **Empty State & Refresh:** When all tours are removed, it displays a message and a button to fetch the tours again.
* **Responsive Design:** The layout adapts to different screen sizes (using CSS media queries).

## Technologies Used

* React.js (using Hooks: `useState`, `useEffect`)
* JavaScript (ES6+ including `async/await` and `fetch`)
* CSS3 (with Custom Properties/Variables)

## Project Setup

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd <repository-directory-name>
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    # or
    # yarn install
    ```

## Running the Project

* **Development Mode:**
    ```bash
    npm run dev
    # or if using Create React App:
    # npm start
    ```
    This will typically start the development server and open the application in your default browser (e.g., `http://localhost:5173` or `http://localhost:3000`).

## API Used

This project fetches data from the following endpoint provided by `course-api.com`:
`https://www.course-api.com/react-tours-project`

## Project Structure

* **`src/App.jsx`:** Main component, handles fetching data, managing loading state, and passing data/functions down.
* **`src/Tours.jsx`:** Component responsible for rendering the list of `Tour` components.
* **`src/Tour.jsx`:** Component representing a single tour card, handling "Read More/Less" and the "Not Interested" button logic.
* **`src/Loading.jsx`:** Simple component to display the loading indicator.
* **`src/index.css` (or similar):** Contains global CSS and specific styles for the components.

## Potential Future Improvements

* Implement more robust error handling for the API fetch request.
* Add filtering or sorting options for the tours.
* Enhance the UI/UX with animations or transitions.
* Consider using a state management library (like Context API or Zustand) if the application were to grow larger.

