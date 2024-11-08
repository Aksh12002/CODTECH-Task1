**Name:** Akshay Parshuram Bagul
**Company:** CODTECH IT SOLUTIONS
**Domain:** CYBER SECURITY & ETHICAL HACKING
**Duration:** October- December 2024
**Mentor:** Neela Santhosh

### Project Overview: Advanced Password Strength Checker

The Advanced Password Strength Checker project is a tool designed to assess the robustness of user-entered passwords. By analyzing various factors like **length**, **complexity**, **uniqueness**, and **entropy**, it aims to provide detailed feedback on password strength and suggest improvements, helping users create more secure passwords. This project could be an essential component in applications that require high-security standards, such as online accounts, corporate systems, and secure databases.

#### 1. Project Objectives
The primary goals of this project include:
- **Evaluating Password Security**: Use specific criteria to determine the strength of a password.
- **Improving Password Quality**: Give actionable feedback to help users improve password complexity and randomness.
- **Preventing Weak Password Usage**: Detect common and predictable passwords, discouraging their use to enhance security.
  
#### 2. Core Features and Functionalities
The Password Strength Checker offers the following core functionalities:

1. **Length Validation**:
   - Ensures that the password meets a minimum acceptable length for security.
   - Suggests a longer password if the length is insufficient, with recommendations for a minimum of 8 characters and ideally 12+ characters.

2. **Complexity Validation**:
   - Analyzes the password for the presence of different character types:
     - **Lowercase Letters**: Ensures a mix of lowercase letters for improved randomness.
     - **Uppercase Letters**: Adds an extra layer of complexity.
     - **Numbers**: Encourages the inclusion of numeric characters to make the password harder to guess.
     - **Special Characters**: Looks for symbols like `@`, `#`, `$`, etc., which increase the password's unpredictability.

3. **Uniqueness Check**:
   - **Blacklist Validation**: Checks the password against a list of commonly used passwords that are often weak (e.g., "123456", "password", "qwerty"). If the password is on this list, users are warned to avoid these predictable options.
   - **Entropy Calculation**: The password entropy is calculated based on its length and character variety. Higher entropy indicates greater password strength, as it suggests a higher degree of randomness.

4. **Detailed Feedback**:
   - Provides the user with a strength rating, such as "Very Weak," "Weak," "Moderate," "Strong," or "Very Strong."
   - Supplies specific recommendations based on detected weaknesses, helping users improve password security. Feedback might include suggestions to add special characters, make the password longer, or avoid using common patterns.

5. **Loop Functionality**:
   - Allows the user to check multiple passwords in one session, providing feedback for each one entered until they decide to exit. This can be useful for users testing different password options.

#### 3. Technical Implementation

This project is implemented in Python, utilizing standard libraries such as:
- **Regular Expressions (`re`)**: Used to validate and locate specific character patterns in passwords.
- **Math (`math.log2`)**: Used to calculate entropy, assessing the randomness and security level of the password.

The tool breaks down password strength into individual components, giving each a score based on criteria. The final strength rating is then calculated based on these scores.

#### 4. Algorithm and Design Approach

The tool follows a step-by-step approach to assess and evaluate each password:

1. **Receive Input**: Prompt the user for a password, allowing for multiple checks in one session.
2. **Character Analysis**:
   - Check if the password includes lowercase letters, uppercase letters, numbers, and special characters.
   - For each character type present, increment the score and skip recommendations related to that type.
3. **Length and Entropy Evaluation**:
   - Measure the password length and add it to the overall score if it meets secure standards (8+ characters, ideally 12+).
   - Calculate the password's entropy to gauge unpredictability. If entropy is low, it suggests that the password is too predictable.
4. **Common Password Check**:
   - Compare the entered password against a blacklist of known weak passwords. If a match is found, the tool warns the user and reduces the score.
5. **Provide Feedback**:
   - Based on the evaluations, output the password’s strength rating, entropy score, and specific improvement suggestions.

#### 5. Expected Output

Each password entered will generate an output detailing:
- **Strength Rating**: Ranging from "Very Weak" to "Very Strong."
- **Entropy Score**: A numerical value indicating the randomness or predictability of the password.
- **Issues and Feedback**: If the password does not meet certain criteria, specific suggestions are given (e.g., “Add uppercase letters,” “Include special characters,” or “Avoid common passwords”).

#### 6. Example Use Cases

The Password Strength Checker is suitable for a range of applications:
- **Web and Mobile Applications**: Encourage users to create strong passwords during registration.
- **Corporate Security Systems**: Help employees set passwords that meet organizational security standards.
- **Educational Tools**: Demonstrate good password practices and educate users on password security principles.

#### 7. Potential Future Enhancements

To further improve the project, additional features could be implemented, such as:
- **Dictionary Attack Detection**: Integrate a dictionary-based check to catch common words, which would discourage using words easily found in English or other language dictionaries.
- **Enhanced Blacklist**: Expand the blacklist by integrating with databases of leaked passwords (e.g., Have I Been Pwned?).
- **Graphical UI**: Build a graphical user interface for ease of use, particularly helpful in desktop or web applications.
- **Advanced Entropy Calculations**: Consider methods that account for repeated character patterns, keyboard patterns (e.g., "qwerty"), and commonly used words (e.g., "password123").

#### 8. Conclusion

This Password Strength Checker project provides a comprehensive tool for evaluating password security. By guiding users in creating stronger, more secure passwords, it contributes to improved security practices and awareness. With future enhancements, it has the potential to become an even more robust tool for password evaluation and feedback.
