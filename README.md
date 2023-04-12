# text_finder_and_coordinates_from_pdf
This Python code searches for text in a PDF file, extracts rectangles containing the text using PyMuPDF and OpenCV libraries, and uses Hugging Face Transformers library to answer questions based on contextual information. The tool is useful for quick extraction of relevant information from PDF files.

This Python code searches for specific text within a PDF file and extracts the coordinates of any rectangles that contain the text. The code first uses the PyMuPDF library to open the PDF file and check each page for the search text. If found, it converts that page to a PNG image using the pdf2image library and applies the Canny edge detection algorithm and contour detection to identify any rectangular areas around the text. The OpenCV library is used to draw rectangles around these areas on the image and save it as a new PNG file.

The code then uses the Hugging Face Transformers library to create a natural language processing (NLP) pipeline that can answer questions based on contextual information. It prompts the user to enter a question, and then uses this NLP pipeline to search for answers within each text block on the page. If an answer is found, the code records the page number, rectangle number, and coordinates of the rectangle in a CSV file, along with the corresponding answer.

Overall, this code provides a useful tool for quickly finding and extracting relevant information from PDF files.
