# Online Collage Editor

Welcome to the Online Collage Editor! This application allows users to create custom collages from uploaded images with flexible options. Below you'll find instructions on how to use the application and details about its functionality.

## Features

- **Image Upload**: Users can upload images without registration.
- **Collage Orientation**: Choose between creating a horizontal or vertical collage.
- **Customization Options**: Define the border size and color for your collage.
- **Asynchronous Processing**: Collage creation is processed asynchronously, allowing users to continue interacting with the application while their collage is being made.
- **Downloadable Collages**: After processing, users can download their final collage.

## How to Use

### 1. Upload Images
- No registration is required.
- Simply upload the images you want to include in your collage.

### 2. Choose Collage Type
- **Horizontal Collage**: Resizes images to the same height while maintaining aspect ratio.
- **Vertical Collage**: Resizes images to the same width while maintaining aspect ratio.

### 3. Customize Your Collage
- **Border Size**: Specify the thickness of the borders between images.
- **Border Color**: Choose a color for the borders.

### 4. Create Your Collage
- Click on the “Make Collage” button.
- The front-end will call the API to start the processing job.
- A loading screen will be shown while the collage is being created.

### 5. Check Processing Status
- The front-end can query the backend API to check if the collage processing is complete.

### 6. Download Your Collage
- Once the processing is finished, you will be redirected to a page where you can download your final collage.

## Technical Details

### Image Resizing
- **Horizontal Collage**: Images are resized to the same height. Aspect ratios are preserved.
- **Vertical Collage**: Images are resized to the same width. Aspect ratios are preserved.

### Collage Creation
- Resized images are stitched together with the user-defined borders.
- Border customization allows for both size and color adjustments.

### Asynchronous Processing
- Image processing is handled asynchronously using a task queue.
- Users are shown a loading screen while their collage is being prepared.

## API Endpoints

- **Upload Image**: Endpoint for uploading images.
- **Start Collage Processing**: Endpoint for initiating the collage creation.
- **Check Processing Status**: Endpoint to query the status of the collage processing job.
- **Download Collage**: Endpoint for downloading the completed collage.

## Example Workflow

1. User uploads multiple images.
2. User selects a horizontal or vertical collage, sets border size and color.
3. User clicks “Make Collage”.
4. A loading screen appears while the collage is being processed.
5. User checks the status until processing is complete.
6. User is redirected to a download page once the collage is ready.


