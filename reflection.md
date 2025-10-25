# Reflection

## 1. Which issues were the easiest to fix, and which were the hardest? Why?

The easiest issues to fix were the formatting and style violations reported by **Flake8** and **Pylint**, such as adding missing blank lines, renaming functions to follow the `snake_case` naming style, and replacing old-style `%` formatting with **f-strings**. These changes were straightforward and instantly made the code more readable.

The hardest issues were removing the **global statement** and replacing the bare `except:` with specific exception types. These required a deeper understanding of how data was being managed and how exceptions could occur, so they took more time and testing to ensure the program still worked correctly.

---

## 2. Did the static analysis tools report any false positives? If so, describe one example.

No major false positives were found during the analysis. All the issues reported by **Pylint**, **Flake8**, and **Bandit** were valid and useful. Some minor warnings, such as those related to blank lines or line length, did not affect the functionality of the code but still helped make the code more consistent and easier to read.

---

## 3. How would you integrate static analysis tools into your actual software development workflow?

I would integrate **Pylint**, **Flake8**, and **Bandit** into a **Continuous Integration (CI)** pipeline using **GitHub Actions** so that these tools automatically check for issues whenever code is pushed or a pull request is created. This ensures that no code with security or style issues gets merged into the main branch.  
I would also use **pre-commit hooks** locally to run these tools before committing any changes, so potential problems are caught early in development.

---

## 4. What tangible improvements did you observe in the code quality, readability, or potential robustness after applying the fixes?

After applying the fixes, the code became much cleaner and easier to understand. Consistent naming conventions, proper indentation, and added **docstrings** improved readability.  
The removal of **eval()** and the use of proper **exception handling** made the program more secure and robust.  
Using **encoding** in file operations and removing the **global variable** dependency improved maintainability.  
Overall, the final version of the program was safer, more efficient, and achieved a perfect **Pylint score of 10/10**.
