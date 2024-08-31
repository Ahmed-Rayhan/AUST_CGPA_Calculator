# CGPA Calculator Web Application

This is a simple web application that allows users to calculate their Cumulative Grade Point Average (CGPA) based on their course marks and credit hours. The app is built using HTML, CSS, and JavaScript and is designed to be user-friendly and easily extendable.

## Features

- **Dynamic Course Input:** Users can add multiple courses by clicking the "Add Another Course" button. 
- **Grade Calculation:** The application calculates the grade points based on a predefined grading system.
- **CGPA Calculation:** The app computes the CGPA by considering the marks and corresponding credit hours for each course.
- **Responsive Design:** The app is designed to be responsive and user-friendly on various devices.

## Grading System

The following grading system is used to calculate grade points:

| Marks Range        | Grade | Point |
|--------------------|-------|-------|
| 80% and above      | A+    | 4.00  |
| 75% to less than 80%| A    | 3.75  |
| 70% to less than 75%| A-   | 3.50  |
| 65% to less than 70%| B+   | 3.25  |
| 60% to less than 65%| B    | 3.00  |
| 55% to less than 60%| B-   | 2.75  |
| 50% to less than 55%| C+   | 2.50  |
| 45% to less than 50%| C    | 2.25  |
| 40% to less than 45%| D    | 2.00  |
| Less than 40%      | F     | 0.00  |

## Project Structure

- **`index.html`**: The main HTML file containing the structure and content of the web application.
- **`style.css`**: Contains custom CSS styles for the web application (if separated).
- **`script.js`**: JavaScript file handling the logic for adding courses and calculating CGPA (if separated).
- **`README.md`**: This file, explaining the project and its structure.

## How It Works

1. **Input Courses:** The user inputs their marks and credit hours for each course. The "Add Another Course" button allows the user to dynamically add more courses.
   
2. **Grade Calculation:** When the user submits the form, the application calculates the grade points for each course using the following formula:
Grade Points = Marks * Credits

The grade points are determined by the `getGrade(marks)` function.

3. **CGPA Calculation:** The total grade points are summed and divided by the total credit hours to calculate the CGPA:
CGPA = Total Grade Points / Total Credits


4. **Display Result:** The calculated CGPA is displayed to the user on the screen.

## Code Explanation

- **HTML:** The HTML structure includes a form with dynamically generated input fields for marks and credits. Each course's marks and credits are entered in corresponding input fields.

- **CSS:** Basic styling is applied to ensure a clean, user-friendly interface. Flexbox is used to align the marks and credits input boxes, with the credit box being smaller (25% of the marks box width).

- **JavaScript:**
- `getGrade(marks)`: A function that returns the grade point based on the input marks.
- `calculateCGPA(marks, credits)`: A function that calculates the CGPA using the grade points and credit hours.
- `addCourse()`: A function that dynamically adds new course input fields to the form.
- The form submission event listener calculates and displays the CGPA when the form is submitted.

## Usage

1. Open the `index.html` file in your web browser.
2. Enter your marks and corresponding credit hours for each course.
3. Click "Add Another Course" to add more courses if needed.
4. Click "Calculate CGPA" to see your CGPA displayed on the screen.

## Customization

You can customize the grading system, styling, or add new features by modifying the respective sections in the code.

## License

This project is open-source and available under the [MIT License](LICENSE).

