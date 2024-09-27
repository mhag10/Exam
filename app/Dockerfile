# Use an official Python runtime as a parent image
FROM python:3.10

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . .

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt 

# Make port 8000 available to the world outside this container
EXPOSE 8000

# Define environment variable (Optionally can pass from runtime)
ENV GROQ_API_KEY="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"

# Run the FastAPI application using Uvicorn
CMD ["python", "uvicorn", "mini_groq:app", "--host", "0.0.0.0", "--port", "8000"]
