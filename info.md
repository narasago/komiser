The following are the things to be taken care when developing new services for other platforms
Backend:

    Create a new service for Azure here: https://github.com/mlabouardy/komiser/tree/master/services
    On the service folder, declare each Azure service on its own file (for e.g: AWS S3 service: https://github.com/mlabouardy/komiser/blob/master/services/aws/s3.go)
    Define the Azure service model (structs) here: https://github.com/mlabouardy/komiser/tree/master/models (for e.g: AWS bucket model: https://github.com/mlabouardy/komiser/blob/master/models/aws/bucket.go)
    Once the Azure service logic is implemented, define the REST API endpoint here: https://github.com/mlabouardy/komiser/tree/master/handlers (for e.g: AWS S3 API endpoints: https://github.com/mlabouardy/komiser/blob/master/handlers/aws/s3_handler.go)
    Finally, expose those endpoints in API route handler: https://github.com/mlabouardy/komiser/blob/master/main.go

For the UI, it’s an Angular project, you find the instructions here: https://github.com/mlabouardy/komiser/tree/master/dashboard

