# Image Colorizer

A web application that uses deep learning to colorize black and white images. Built with Next.js for the frontend and Python with OpenCV for the colorization process.

![Image Colorizer](https://github.com/username/image-colorizer/raw/main/public/placeholder.jpg)

## Features

- Upload black and white images
- Automatic colorization using a pre-trained deep learning model
- Download colorized images
- Modern, responsive UI

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or later)
- [Python](https://www.python.org/) (v3.6 or later)
- [Git](https://git-scm.com/)
- [OpenCV](https://opencv.org/) for Python

## Setup Instructions

### 1. Clone the repository

```bash
# Clone this repository to your local machine
git clone https://github.com/your-username/image-colorizer.git

# Navigate to the project directory
cd image-colorizer
```

### 2. Install Node.js dependencies

```bash
npm install
```

### 3. Set up Python environment

```bash
# Install required Python packages
pip install numpy opencv-python
```

### 4. Download the pre-trained model

Download the pre-trained model file from the following link and place it in the `Colorizing-black-and-white-images-using-Python-master/model/` directory:

[Download colorization_release_v2.caffemodel](https://www.dropbox.com/s/dx0qvhhp5hbcx7z/colorization_release_v2.caffemodel?dl=1)

### 5. Create required directories

Ensure the following directories exist for storing uploaded and colorized images:

```bash
mkdir -p public/uploads public/colorized
```

## Running the Application

### Development mode

```bash
npm run dev
```

This will start the Next.js development server at [http://localhost:3000](http://localhost:3000).

### Production mode

```bash
# Build the application
npm run build

# Start the production server
npm start
```

## Deploying to GitHub

1. Create a new repository on GitHub

2. Initialize Git in your project (if not already done)
   ```bash
   git init
   ```

3. Add your files to Git
   ```bash
   git add .
   ```

4. Commit your changes
   ```bash
   git commit -m "Initial commit"
   ```

5. Add your GitHub repository as a remote
   ```bash
   git remote add origin https://github.com/your-username/image-colorizer.git
   ```

6. Push your code to GitHub
   ```bash
   git push -u origin main
   ```

## Project Structure

- `/app` - Next.js application code
  - `/api` - API routes for image processing
  - `/components` - React components
- `/public` - Static assets and processed images
- `/Colorizing-black-and-white-images-using-Python-master` - Python colorization code
  - `/model` - Pre-trained model files

## How It Works

1. User uploads a black and white image through the web interface
2. The image is sent to the Next.js API endpoint
3. The API saves the image and calls the Python script
4. The Python script uses a pre-trained deep learning model to colorize the image
5. The colorized image is saved and returned to the frontend
6. The user can view and download the colorized image

## Technologies Used

- **Frontend**: Next.js, React, Tailwind CSS
- **Backend**: Next.js API Routes
- **Image Processing**: Python, OpenCV, Caffe model
- **Styling**: Tailwind CSS, Radix UI components

## Acknowledgements

- [Colorizing black and white images using Python](https://github.com/richzhang/colorization) - Original colorization model
- [Next.js](https://nextjs.org/) - The React framework
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework
- [Radix UI](https://www.radix-ui.com/) - UI component library
