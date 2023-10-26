# Backend

The backend of our application serves as the core engine, responsible for managing requests from the frontend, processing data, and interacting with the database.

## Technologies Used

- **Node.js**: JavaScript runtime for server-side development.
- **Express.js**: Web application framework for Node.js, simplifying API development.
- **AWS S3**: Cloud storage service for storing and retrieving images.
- **MongoDB**: NoSQL database for efficient and scalable data storage.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB and Node.js.

## Getting Started

1. **Clone the Repository**: Begin by cloning the repository to your local machine.
2. **Install Dependencies**: Use `npm install` to install all necessary dependencies.
3. **Set Up Environment Variables**:
   - Create a `.env` file in the project root.
   - Add the following environment variables:
     - `MONGODB_URI`: URI for your MongoDB database.
     - `AWS_ACCESS_KEY_ID`: Your AWS access key ID.
     - `AWS_SECRET_ACCESS_KEY`: Your AWS secret access key.
     - `AWS_REGION`: The region where your S3 bucket is located.
     - `AWS_BUCKET_NAME`: The name of your S3 bucket.
4. **Start the Server**: Initiate the server using `npm start`.

## Endpoints

### POST /api/upload

This endpoint facilitates image uploads to the S3 bucket. The request must include a `multipart/form-data` body containing an `image` field. Upon successful upload, the response will contain the URL of the uploaded image.

Example Request:
```http
POST /api/upload
Content-Type: multipart/form-data

[image: image_file]
```

Example Response:
```json
{
  "imageUrl": "https://s3.amazonaws.com/bucket_name/image_file.jpg"
}
```

[Note: Provide appropriate image file and bucket name in the request]

---

**Note**: Ensure that you have the necessary permissions and configurations set up both for AWS S3 and MongoDB to enable seamless functioning of the backend.