# Lab-5-202001203

Static Analysis Tool Used: Pylint
Language: Python

                                                                    File 1 Name: watermark.py

![image](https://user-images.githubusercontent.com/75676773/225587792-7a9a7200-f8d1-436c-bb8b-fb57cd11c18c.png)

**– ANALYSIS –**

**Error 1:** watermark.py:45:0: C0305: Trailing newlines (trailing-newlines)

There is a trailing newline at the end of line 45 in this file. This means that there is an extra blank line after the last line of code in that file, which is considered bad style in Python.

**Solution:** Remove the extra blank line at the end of the file or block of code.

**Error 2:** watermark.py:1:0: C0114: Missing module docstring (missing-module-docstring)

It indicates that the module-level docstring is missing in this file. A docstring is a string literal that appears as the first statement in a module, function, class, or method definition. Its purpose is to provide a concise description of what the code does and how it should be used.

**Solution:** Add a module-level docstring to the "watermark.py" file.

**Error 3:** watermark.py:2:0: E0401: Unable to import 'PIL' (import-error)

It indicates that there was a problem importing the 'PIL' module in the 'watermark.py' file i.e. 'PIL' module may not be installed or it may not be in the Python path. PIL stands for Python Imaging Library, which is a library used for opening, manipulating and saving many different image file formats.

**Solution:** PIL module can be installed using pip command: **pip install Pillow**

**Error 4:** watermark.py:4:0: C0116: Missing function or method docstring (missing-function-docstring)

It indicates that the docstring is missing for a function or method defined in this file.

**Solution:** Add a docstring to the function or method in question. The docstring should describe the purpose of the function or method and any relevant information about how it should be used.

**Error 5:** watermark.py:6:4: W0621: Redefining name 'watermark' from outer scope (line 32) (redefined-outer-name)

This error message is related to a specific warning in Python called W0621. I indicates that the name 'watermark' is being redefined in a nested scope, and that this may cause unexpected behavior in the code. In Python, a variable defined in an inner scope with the same name as a variable in an outer scope will override the outer variable. This can lead to unintended consequences if the outer variable is still needed in the code.

**Solution:** Use a different variable name in the nested scope to avoid overriding the outer variable. 

**Error 6:** watermark.py:40:0: C0103: Constant name "c" doesn't conform to UPPER_CASE naming style (invalid-name)

There is a problem with a constant named "c" in line 40 of this file. Name of the constant "c" does not conform to the UPPER_CASE naming style.
In Python, it is a convention to use all capital letters to name constants. This helps to distinguish constants from other types of variables and makes the code easier to read.

**Solution:** rename the constant "c" to use all capital letters, camelCase or snake_case.

                                                           File 2 Name: convert_image_to_pdf.py

![image](https://user-images.githubusercontent.com/75676773/225584154-481e9f4e-c765-42d2-875a-7bd9a9dd4ba8.png)

**– ANALYSIS –**

**Error 1:** convert_image_to_pdf.py:23:0: C0305: Trailing newlines (trailing-newlines)
It indicates that there are trailing newlines at the end of the file or the line specified in the error message (line 23 in this file).

Trailing newlines refer to empty lines that appear at the end of a file or code block.

**Solution:** Remove any extra empty lines or spaces at the end of the file or line mentioned in the error message. This should resolve the trailing-newlines issue and clear the Pylint warning.

**Error 2:** convert_image_to_pdf.py:1:0: C0114: Missing module docstring (missing-module-docstring)

The error message is indicating that the module convert_image_to_pdf.py is missing a docstring. A docstring is a string that appears at the beginning of a module, function, class, or method definition that describes what the module, function, class, or method does.

Pylint considers it a best practice to include a docstring in every module, as it helps make the code more readable and maintainable.

**Solution:** Add a docstring to the beginning of the module.

**Error 3:** convert_image_to_pdf.py:2:0: E0401: Unable to import 'img2pdf' (import-error)

It indicates that there is an import error in the file 'convert_image_to_pdf.py' when attempting to import the module 'img2pdf'.

An import error occurs when Python is unable to locate the module that is being imported, or when there is an issue with the module itself.

**Solution:** Activate the correct environment and install the img2pdf module using pip, by running the command pip install img2pdf in your command prompt or terminal.

**Error 4:** convert_image_to_pdf.py:5:0: C0103: Constant name "filepath" doesn't conform to UPPER_CASE naming style (invalid-name)

It indicates that the variable filepath in the file convert_image_to_pdf.py does not conform to the UPPER_CASE naming style that is commonly used for constants in Python. 

In Python, constants are typically defined using all capital letters with underscores separating words. This convention helps to differentiate constants from variables and makes it clear that the value of the constant should not be changed during runtime.

**Solution:** Rename the variable filepath to FILE_PATH or a similar name that follows the UPPER_CASE naming style convention.

**Error 5:** convert_image_to_pdf.py:3:0: C0411: standard import "import os" should be placed before "import img2pdf" (wrong-import-order)

It indicates that in this file, the standard library module os should be imported before the third-party library 'img2pdf'. Standard library modules are typically more stable and less likely to change than third-party libraries. By importing standard library modules first, it can help to identify any potential namespace conflicts with third-party libraries.

**Solution:** Move the import statement for **os** above the import statement for **img2pdf**.
