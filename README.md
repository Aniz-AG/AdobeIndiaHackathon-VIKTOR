Adobe India Hackathon 2025: Connecting the Dots
✨ Welcome to the “Connecting the Dots” Challenge

🔍 Rethink Reading. Rediscover Knowledge.

Imagine this: every time you open a PDF, it doesn’t just passively display information — it speaks to you, highlights important ideas, draws intelligent connections, and becomes your research co-pilot. That’s the future we’re building. That’s the vision behind Connecting the Dots. And we want you to shape it.

In this challenge, you’ll reimagine the humble PDF as a smart, interactive, AI-powered reading experience. One that understands structure, connects concepts, and learns with you — just like a human collaborator.

🗺️ The Journey Ahead
This challenge consists of two exciting rounds, each designed to test and showcase your ability to merge intelligence with innovation.

🔹 Round 1: Build the Brain 🧠
This round is divided into two parts, focusing on core functionality and intelligent analysis.

Round 1A: Understand Your Document: Your mission is to build a solution that extracts a structured outline (Title, H1, H2, H3) from raw PDFs with high speed and accuracy. This forms the foundational layer of document intelligence. 





Round 1B: Persona-Driven Document Intelligence: Building on Round 1A, you will create a system that analyzes a collection of documents to extract and prioritize sections relevant to a specific user persona and their task. 



🔹 Round 2: Design the Experience 💡
It's time to bring your smart PDF engine to life! In this round, you will build a sleek, modern, and intuitive web application using 

Adobe's PDF Embed API, integrating the intelligence from Round 1 to create a magical and interactive reading experience. 

🌍 Why This Challenge Matters
In today's world, we're drowning in documents. The problem isn’t 

access to content — it’s understanding it. This challenge is about creating a 


new reading paradigm by building tools that offer context, clarity, and insight. 

Whether you're a:
👩‍💻 Machine learning engineer
🎨 UI/UX designer
📊 Data wrangler
🧙 Insight whisperer

This is your opportunity to lead the evolution of knowledge interfaces.

🧩 Challenge Solutions
Below are the core solution components you’ll be working with.

✅ Challenge 1A: PDF Outline Extraction
A Dockerized solution that accepts a PDF file and outputs a structured JSON file containing the document's title and hierarchical headings (H1, H2, H3) with their respective page numbers. 



Tech Stack:

Containerization: Docker

PDF Processing: Python with libraries like PyMuPDF (fitz) or pdfplumber for text and metadata extraction.

Logic/ML: Rule-based algorithms (analyzing font size, style, and positioning) or a lightweight ML model (e.g., trained with scikit-learn) for heading classification. The model size must be 

≤ 200MB. 

How to Run the Code:

Build the Docker Image:
Place your Dockerfile in the root of your project directory. Then, run the build command:

Bash

docker build --platform linux/amd64 -t mysolutionname:somerandomidentifier .


Your Dockerfile must be compatible with the 

linux/amd64 architecture and should not have GPU dependencies. 


Prepare Input/Output Directories:
Create two folders named input and output in your project directory. Place the PDF files you want to process into the input folder.

Run the Container:
Execute the following command to run your solution. The container will automatically process all PDFs from the 

/app/input directory and save the corresponding JSON files to the /app/output directory. 

Bash

docker run --rm -v $(pwd)/input:/app/input -v $(pwd)/output:/app/output --network none mysolutionname:somerandomidentifier


The entire process must work 

offline without any internet access. 


Constraints:


Execution Time: ≤ 10 seconds for a 50-page PDF. 


Model Size: ≤ 200MB (if a model is used). 


Runtime Environment: CPU only (amd64), 8 CPUs, 16 GB RAM. 

✅ Challenge 1B: Persona-Based Multi-Document Analysis
An advanced Dockerized solution that analyzes a collection of 3-10 PDFs based on a given user persona and a specific "job-to-be-done."  The output is a JSON file containing ranked, relevant sections and sub-sections from the documents.


Tech Stack:

Containerization: Docker

PDF & Text Processing: Python with libraries from Challenge 1A, supplemented by NLP libraries like NLTK or spaCy for text analysis.

Semantic Analysis/ML: Vector-based models (e.g., Sentence-Transformers, spaCy's built-in models) to determine the relevance between document sections and the persona's query. The model size must be 

≤ 1GB. 

How to Run the Code:

Build the Docker Image:
Follow the same Docker build instructions as in Challenge 1A, ensuring your 

Dockerfile and all dependencies are included. 

Run the Container:
Use the execution instructions specified in your README.md file. The command will likely be similar to Challenge 1A but adapted for multiple inputs (documents, persona, job-to-be-done).

Constraints:


Processing Time: ≤ 60 seconds for a collection of 3-5 documents. 


Model Size: ≤ 1GB. 


Runtime Environment: CPU only. 


Network: No internet access is allowed during execution. 

🌟 Let’s Build the Future of Reading
It’s time to:
🔬 Look deeper than the surface
🧩 Connect what’s scattered
🚀 Build experiences that feel like magic

Let’s redefine how the world reads.
Let’s connect the dots.


Are you in? 
