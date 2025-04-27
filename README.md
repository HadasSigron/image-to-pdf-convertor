## Build Image
docker build -t image-to-pdf .
##the run command
docker run -v $(pwd)/images:/app/images -v $(pwd)/output:/app/output -e PDF_NAME=myoutput image-to-pdf images
## or with defult environment variable
docker run -v $(pwd)/images:/app/images -v $(pwd)/output:/app/output image-to-pdf images
