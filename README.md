# CT Head Scan Visualisation

A Java computer graphics project developed as part of my **CS-255 Computer Graphics** module at Swansea University.

The application loads and visualises a three-dimensional CT head dataset, allowing the user to explore medical image data from multiple viewing directions.

I originally developed this project during my Computer Science degree and have retained it on GitHub as an example of my earlier Java and computer graphics work.

## Features

- Loads a raw 3D CT dataset into memory
- Displays CT data from multiple viewing directions
- Implements Maximum Intensity Projection (MIP)
- Allows individual CT slices to be explored using interactive sliders
- Converts raw CT intensity values into greyscale pixel values for display
- Supports image resizing
- Generates thumbnails of CT slices
- Uses mouse and UI events for interaction
- Provides a graphical interface using JavaFX

## Technologies Used

- Java
- JavaFX
- Binary file I/O
- 3D arrays
- PixelReader and PixelWriter
- Event-driven programming
- Computer graphics and image-processing techniques

## How It Works

The CT dataset is represented as a three-dimensional array containing **113 × 256 × 256** intensity values.

The application reads the raw binary CT data into memory and processes the byte order before storing each value in the 3D array.

The minimum and maximum intensity values in the dataset are identified and used to normalise the CT values into greyscale values suitable for displaying as an image.

### CT Slice Viewing

The application can display individual slices of the CT volume from different orientations.

JavaFX sliders allow the user to move through the dataset and view different slices interactively.

### Maximum Intensity Projection

The application implements **Maximum Intensity Projection (MIP)** from multiple viewing directions.

For each output pixel, the program examines values through the corresponding direction of the 3D dataset and selects the maximum intensity value. This produces a two-dimensional projection highlighting high-intensity structures within the CT volume.

### Image Resizing

The project includes image-resizing functionality implemented using coordinate mapping between the source and destination images.

JavaFX `PixelReader` and `PixelWriter` are used to read and write individual pixel values.

### CT Slice Thumbnails

The application can generate smaller thumbnail images representing slices through the CT dataset. These thumbnails are displayed through the JavaFX interface and use mouse-event handling to provide interaction.

## What I Learned

This project gave me practical experience applying Java to a computer graphics problem rather than only working with basic programming exercises.

Some of the key areas I worked with included:

- Working with multidimensional arrays and large datasets
- Reading binary data from files
- Understanding byte ordering and converting raw binary values
- Processing and normalising numerical data for visualisation
- Manipulating individual image pixels
- Implementing Maximum Intensity Projection algorithms
- Working with nested loops for image and volume processing
- Building graphical interfaces with JavaFX
- Using event listeners and UI controls
- Implementing basic image-resizing techniques
- Breaking a larger graphics problem into separate methods and operations

## Background

This project was originally completed during my **BSc Computer Science at Swansea University (2018–2021)** as part of the CS-255 Computer Graphics module.

I am currently refreshing and developing my Java and software development skills and revisiting earlier university projects as part of that process.

## Future Improvements

If I continued developing the project, I would look to:

- Refactor the application into smaller classes with clearer separation of responsibilities
- Replace the hard-coded dataset path with a file-selection interface
- Improve error handling and validation
- Improve the user interface and layout
- Add automated tests where appropriate
- Improve documentation throughout the code
- Review and optimise the image-processing algorithms
- Modernise the project structure and build configuration

## Author

**Fawaz Muhammed**  
BSc Computer Science — Swansea University
