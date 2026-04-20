# handwriten-charachters-recognize-system
A smart handwriting recognition module written in Python and based on the PyQt6 and Tensorflow libraries. It's useful for creating clear, structured notes for school lessons, university lectures, and other events.

Documentation and Project Overview

---

##  Technology Stack

### Frontend
**Interaction Window Widgets:**
1.  **Main Workspace:**
    *   **Drawing Canvas:** Supports mouse or stylus input.
2.  **Toolbar:**
    *   **"Recognize" Button:** Triggers the processing of the current drawing.
    *   **"Clear" Button:** Fully clears the canvas for new input.
    *   **"Add to Text" Button:** Sends the recognized text to the growing notes document.
    *   **"Pen Thickness" Slider:** Adjusts the brush size to match the user's handwriting.
3.  **Text Field:**
    *   Displays the recognized text and allows for manual keyboard corrections.
4.  **Navigation & Saving:**
    *   **"Save Notes" Button:** Exports the accumulated text into a `.txt` file.
    *   **"Upload Image" Button:** Allows uploading photos of handwritten notes for recognition.
5.  **Future Features:**
    *   Integrated Chatbot window.
    *   Neural network confidence indicator.

### Backend
**Architectural Requirements:**
*   Efficient frontend-backend communication.
*   Modular design for easy scalability.

**Core Functionality:**
1.  Loading and running trained neural network models.
2.  Image preprocessing (compression, grayscale conversion, vectorization).
3.  **Application Logic:**
    *   Recognition request handling.
    *   Note management (appending and saving).
    *   File I/O operations for image uploads.
4.  Asynchronous task execution for smooth UI performance.

---

##  Libraries Used (Python)
*   **Tensorflow/Keras:** Model loading and inference.
*   **NumPy:** Numerical operations and array manipulation.
*   **OpenCV:** Image processing and resizing.
*   **PyQt6:** Graphical User Interface (GUI) framework.
*   **Standard Library:** `os` for file system tasks.

---

##  Use Cases
1.  **Direct Recognition:** User draws → clicks "Recognize" → clicks "Add to Text".
2.  **Manual Correction:** User edits recognized text in the output field before saving.
3.  **Exporting:** User saves the entire session as a `.txt` file.
4.  **Batch Processing:** User uploads an existing image for text extraction.
