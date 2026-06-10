🏗️ Steel Weight Calculator
A fast, interactive, browser-based utility originally designed for NISHA STEEL N ALLOYS (Technical Division). This tool calculates the weight, dimensions, and lengths of various industrial steel profiles including rings, round bars, and multi-step shafts.

It is built with pure HTML, CSS, and Vanilla JavaScript, requiring no external dependencies or backend.

✨ Key Features
Ring / Pipe Calculator: Calculate the total weight based on Outer Diameter (OD), Inner Diameter (ID), Thickness, and Material Loss percentage.

Round Bar Calculator: Calculate weight using weight-per-meter (WPM), length, and loss estimates.

Step Shaft (Spindle) Tool: * Forward Calculation: Input up to 4 different ODs and Lengths (LG) to get the total step shaft weight.

Reverse Calculation: Input a target total weight, and the app will proportionally adjust the lengths of existing dimensions, or generate standard descending dimensions (100-80-60-40) if starting from scratch.

Length Finders: Reverse-engineer the required length of Square or Round bars based on a target weight and cross-sectional dimensions.

Modern UI: Features a responsive CSS Grid layout, "glassmorphism" panel styling (backdrop blur), and clean, intuitive input fields.

🧮 Technical Constants & Formulas
The calculator relies on industry-standard material density parameters hardcoded into the calculation logic:

Base Density: 0.00000785 kg/mm³ (Standard density for Mild Steel/Carbon Steel).

Pipe/Ring Constant: 0.0000062 (Derived factor for calculating annular volume and weight efficiently).

🚀 Getting Started
Since this is a front-end only application, installation is instantaneous.

Clone the repository:

Bash
git clone https://github.com/yourusername/steel-weight-calculator.git
Navigate to the directory:

Bash
cd steel-weight-calculator
Run the app:
Simply double-click the index.html (or calc.html) file to open it in any modern web browser (Chrome, Firefox, Safari, Edge).

📂 Project Structure
calc.html — The single-file architecture containing:

<html> layout and structural semantic tags.

<style> block utilizing CSS Variables for easy theming.

<script> block containing the DOM manipulation and mathematical logic.

🛠️ Usage Examples
Calculating a Step Shaft:

Navigate to the STEP SHAFT (SPINDLE) section.

Enter OD_1 = 100, LG_1 = 200.

Enter OD_2 = 80, LG_2 = 150.

Click Calculate to output the combined total weight in kilograms.

Reverse Engineering a Shaft:

Leave all OD and LG fields blank in the Step Shaft section.

Type 500 directly into the Total Wt field.

The script will automatically populate standard descending dimensions and scale them to accurately equal a 500kg shaft.

🤝 Contributing
Contributions, issues, and feature requests are welcome!
If you want to add new materials (e.g., Aluminum, Stainless Steel) or new profiles (Hexagonal bars, I-Beams), feel free to fork this repository and submit a pull request.

Fork the Project

Create your Feature Branch (git checkout -b feature/NewCalculator)

Commit your Changes (git commit -m 'Add Hexagonal Bar logic')

Push to the Branch (git push origin feature/NewCalculator)

Open a Pull Request
