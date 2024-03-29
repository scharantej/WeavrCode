## Design: Flask Application for Problem: Generate a prompt that can be used by a large language model to write a business plan for a web development company.

### HTML Files:
1. **index.html**:
   - Home page of the application.
   - Contains a prompt generation form for the business plan.
2. **results.html**:
   - Displays the prompt generated by the application.
   - Includes a button to download the prompt as a text file.

### Routes:
1. **index**:
   - Handles requests for the home page (index.html).
2. **generate_prompt**:
   - Handles POST requests from the prompt generation form.
   - Gathers information from the form and uses it to generate a prompt using Flask's `render_template` function.
   - Redirects to the 'results' route with the generated prompt.
3. **download_prompt**:
   - Handles GET requests for downloading the generated prompt as a text file.
   - Streams the content of the prompt to the client's browser as a text file.