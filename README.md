# Coordinates-extraction-using-PaddleOCR
# 📌 Project Description

The Color Object Coordinate Retrieval Agent is an AI-powered system that extracts and matches coordinates from two nearly identical images: one containing colored objects and another in grayscale with corresponding coordinate labels. The agent processes a user query specifying a color and retrieves the matching object's coordinates from the grayscale image.

# 🚀 Features

- OCR-based Coordinate Extraction: Uses PaddleOCR to extract numeric coordinates from the grayscale image.

- Color Segmentation: Applies OpenCV with HSV color thresholds to detect colored objects.

- Shape Detection: Identifies object contours in the colored image.

- Coordinate Matching: Utilizes Euclidean distance to associate detected objects with extracted coordinates.

- Natural Language Query Processing: Fine-tunes a T5-small model to understand and process user queries.

📜 Workflow

- Extract Coordinates: OCR is applied to detect and extract coordinate labels from the grayscale image.

- Detect Colored Objects: OpenCV is used to segment colored objects using predefined HSV bounds.

- Match Objects with Coordinates: Euclidean distance is used to associate detected shapes with the extracted coordinates.

- Process User Queries: A T5-small model is fine-tuned on synthetic query data to interpret user input.

- Retrieve and Respond: Given a query like "What are the coordinates of the orange object?", the model identifies the color, finds the corresponding object, and returns its coordinates.
