# STAGE 2
Here is the task assigned during this stage.

```
Objective:
You are to deploy a FastAPI application with a Continuous Integration (CI) and Continuous Deployment (CD) pipeline. You will use an existing template repository, add a missing endpoint, set up a test pipeline, and configure the deployment process. Your application should be served using Nginx.

Repository Template:
Fork the following repository as your starting point: FastAPI Book Project Template

Tasks to Complete:
1. Implement the Missing Endpoint
 Add an endpoint to retrieve a book by its ID:
 Path: /api/v1/books/{book_id}
 The endpoint should return a JSON response containing the book details.
 If the book does not exist, return a 404 Not Found response.
 Do not delete any books from the database.
2. Set Up the CI Pipeline
 The CI pipeline should only run pytest to execute the existing tests.
 The workflow should be triggered on pull requests to the main branch.
 The workflow file must:
 Contain a job named exactly test.
 Fail if there are issues in the application.
 Succeed if the application passes all tests.
3. Set Up the Deployment Pipeline
 On merging a pull request to the main branch, a workflow should trigger a job named exactly deploy.
 If the deploy job runs successfully, your site should automatically be updated with the latest changes.
4. Dockerization Requirement:
 Create a Dockerfile that builds and packages the FastAPI application.
 The Dockerfile should:
 Use an official lightweight Python image as the base.
 Install necessary dependencies for FastAPI.
 Expose the required port and set the appropriate FastAPI entry point.
5. Serve the Application Over Nginx
 Your deployed application should be served using Nginx as a reverse proxy.
 Ensure proper configuration so that API requests are correctly handled by the FastAPI backend.
```

In this task, I forked this this [template](https://github.com/hng12-devbot/fastapi-book-project). Here is the [codebase](https://github.com/oxblixxx/fastapi-book-project) that I forked and modified. The procedure for the deployment can be found in this [blog]()