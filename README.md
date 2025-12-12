# Exam


## Overview

This exam requires you to enhance a **Car App** by working on both its frontend and backend components. The application includes public **GET** routes and protected **POST**, **PUT**, and **DELETE** routes.

Your primary objective is to improve the app's models and functionality. Key details include:

- **Model Variations:** There are **four versions** of the Car and User models (A, B, C, or D). These models are available [here](./material/models.md).  
- **Your Assignment:** The specific model assigned to **you** can be found [here](./material/Exam.png).

### Exam Structure

The exam consists of **six iterations** (total: 270 points):

- **Iteration 0 (Setup):** 10 points  
- **Iteration 1:** 60 points  
- **Iteration 2:** 50 points  
- **Iteration 3:** 50 points  
- **Iteration 4:** 50 points  
- **Iteration 5:** 50 points  

Iteration 0 is a short preparatory task to ensure your environment is ready. Iterations 1–5 are the main graded tasks.

### Exam Guidelines

To ensure fairness and consistency:

- All work must be committed and pushed to GitHub within **two hours** of the exam start.
- External monitors are not allowed. Use only your laptop’s built‑in screen.

**Exam Recording Instructions**

- *Recording Requirement*: The coding session must be recorded on your local machine.  
- *Retention Period*: Do not delete the recording until **17th of December**.  
- *Possible Review Situations*: I may request your recording if:  
  - You do not push to GitHub immediately after committing an iteration.  
  - I suspect the use of coding agents.  
  - There is noticeable similarity in code submissions.  
- *How to Record*: Follow the steps outlined in [Recording with Zoom](./material/recording.md). We will review these instructions together before starting the exam.  


**Commit and Push Every Change**

To ensure proper grading:
- At the end of each iteration, make a **commit** with the message format:  
  ```
  [iteration X]: <points> graded
  ```
  where **X** is the iteration number.  
- Immediately run `git push` to upload your changes.  
- Verify that your commits appear in the remote repository.  
- Failure to push commits may result in incomplete grading.

---

### Iteration 0: **10 points**

This iteration focuses on setting up the development environment and ensuring the app runs successfully. Follow these steps carefully:

1. **Clone the Starter Repository**  
   - Clone the [starter code](https://github.com/tx00-web-en/exam-starter) repository and name it `exam-web-dev` as follows: 
     ```bash
     git clone https://github.com/tx00-web-en/exam-starter exam-web-dev
     ```
   - Navigate to the `exam-web-dev` directory and remove the `.git` folder. 


2. **Set Up the Backend**
   - Navigate to the `backend` directory. 
   - Rename `.env.example` to `.env`.
   - Install the necessary dependencies:
      ```sh
      npm install express dotenv cors mongoose jsonwebtoken bcryptjs colors validator cross-env
      ```
   - Install Dev Dependencies
      ```sh
      npm install nodemon jest supertest -D
      ```
   - Run the tests to **ensure** all provided tests **pass**:  
      ```sh
      npm test
      ```      
   - Start the backend server:
     ```sh
     npm run dev
     ```

3. **Set Up the Frontend**  
   - Navigate to the `frontend` directory.  
   - Install the necessary dependencies and start the frontend application:
     ```sh
     npm install
     npm run dev
     ```

4. **Access the App**  
   -  Open [http://localhost:3000](http://localhost:3000) in your web browser to verify the app is running successfully.

5. **Push Your Work to a Private GitHub Repository**  
   - Start by initializing a Git repository in the `exam-starter` project folder:  
     ```sh
     git init
     git add .
     git commit -m "[iteration 0]: grade 10 out of 10 points"
     ```  
   - **Push your changes to GitHub**:  
     - Create a **private** GitHub repository named `exam-web-dev`.  
     - Add the user `55d41251` as a collaborator to your repository.
     - **Important**:  Failure to push your commits may result in incomplete grading.

### Iteration 1:  **60 points**

> **Note:** Each iteration is graded separately. Before starting this iteration, **ensure** that you have made a **commit for the previous iteration and pushed it to GitHub**.


1. **Modify the Backend: 30 Points**  
   - Update the `Car` model according to your assigned model variation (A, B, C or D). 
   - **Test the updated backend functionality using Postman**.

2. **Update the Frontend: 30 Points**  
   - Ensure that the frontend is compatible with the updated backend by making any necessary modifications.

3. **Self-Assessment and Commit**  
   - Create a **commit** in your Git repository that includes the iteration status and your **self-assessed score** for **this iteration only**, out of **50 points**. 
   - To receive the **maximum points**, your code must **work as intended**, and run **without crashing**. 
   - **Example** *commit message*:  
     ```  
     [iteration 1]: grade 20 out of 60 points
     ```  

4. **Push Changes to GitHub**  
   - Push the updated code to your GitHub repository.
   - **Important**: Failure to push your commits may result in incomplete grading.

### Iteration 2:  **50 points**

> **Note:** Each iteration is graded separately. Before starting this iteration, **ensure** that you have made a **commit for the previous iteration and pushed it to GitHub**.


1. **Update the `User` Model: 20 Points**  
   - Modify the `User` model according to the specification for your assigned group (A, B, C or D) and test it with Postman.

2. **Password Validation: 10 Points**  
   - Implement strong password validation using the [validator library](https://www.npmjs.com/package/validator) (e.g., isStrongPassword) to check for password strength.  

3. **Frontend Integration: 20 Points**  
   - Make necessary updates to the frontend to ensure compatibility and seamless functionality with the updated backend.  

4. **Self-Assessment and Commit**  
   - Create a **commit** in your Git repository that includes the iteration status and your **self-assessed score** for **this iteration only**, out of **50 points**. 
   - To receive the **maximum points**, your code must **work as intended**, and run **without crashing**.    
   - **Example** *commit message*:  
     ```  
     [iteration 2]: grade 20 out of 50 points
     ```  

5. **Push Changes to GitHub**  
   - *Push the updated code to your GitHub repository*.
   - **Important**: Failure to push your commits may result in incomplete grading.

### Iteration 3:  **50 points**

> **Note:** Each iteration is graded separately. Before starting this iteration, **ensure** that you have made a **commit for the previous iteration and pushed it to GitHub**.

1. **Update the Test Cases**  
   - Modify the `users` test cases to align with the updated API (**25 Points**).
   - Adjust the `cars` test cases to ensure compatibility with the modified API (**25 Points**).

2. **Self-Assessment and Commit**  
   - Create a **commit** in your Git repository that includes the iteration status and your **self-assessed score** for **this iteration only**, out of **50 points**. 
   - To receive the **maximum points**, your code must **work as intended**, and run **without crashing**.    
   - **Example** *commit message*:  
     ```  
     [iteration 3]: grade 20 out of 50 points
     ```  

3. **Push Changes to GitHub**  
   - *Push the updated code to your GitHub repository.*
   - **Important**: Failure to push your commits may result in incomplete grading.

### Iteration 4:  **50 points**

> **Note:** Each iteration is graded separately. Before starting this iteration, **ensure** that you have made a **commit for the previous iteration and pushed it to GitHub**.

1. **Fix the Login Issue:**  
   - The frontend application currently crashes when incorrect login credentials are entered.  
   - Update the relevant code so that incorrect login attempts are handled gracefully.  
   - A graceful solution should:  
     - Prevent the application from crashing.  
     - Provide a clear error message to the user (e.g., “Invalid credentials”).    
   - If you cannot fully fix the issue, implement a partial solution that ensures the app does not crash and communicates the error appropriately.  


2. **Self-Assessment and Commit**  
   - Create a **commit** in your Git repository that includes the iteration status and your **self-assessed score** for **this iteration only**, out of **50 points**. 
   - To receive the **maximum points**, your code must **work as intended**, and run **without crashing**.     
   - **Example** *commit message*:  
     ```  
     [iteration 4]: grade 20 out of 50 points
     ```  

3. **Push Changes to GitHub**  
   - *Push the updated code to your GitHub repository.*
   - **Important**: Failure to push your commits may result in incomplete grading.

### Iteration 5:  **50 points**

> **Note:** Each iteration is graded separately. Before starting this iteration, **ensure** that you have made a **commit for the previous iteration and pushed it to GitHub**.

1. **Refactor `AddCarPage.jsx`:**
   - In `frontend/src/pages/AddCarPage.jsx`, refactor the current state management for form fields to use the `useField` hook from `frontend/src/hooks/useField.jsx`.
   - Ensure that all form fields (e.g., title, author, etc.) are updated to use the `useField` hook for state management.
   - Verify that the form works correctly after the refactor (ensure fields update, validation works, and form submission behaves as expected).

2. **Self-Assessment and Commit**  
   - Create a **commit** in your Git repository that includes the iteration status and your **self-assessed score** for **this iteration only**, out of **50 points**. 
   - To receive the **maximum points**, your code must **work as intended**, and run **without crashing**.     
   - **Example** *commit message*:  
     ```  
     [iteration 5]: grade 20 out of 50 points
     ```  

3. **Push Changes to GitHub**  
   - *Push the updated code to your GitHub repository.*
   - **Important**: Failure to push your commits may result in incomplete grading.

