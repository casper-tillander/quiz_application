# Quiz Application

## Description

This Quiz Application is an online platform designed to facilitate the creation and answering of quiz questions related to various topics. It is designed to be intuitive and user-friendly, integrating features for both quiz creators and quiz takers. It uses a modern tech stack, has robust security measures in place, and provides an API for third-party integration.

## Features

- **Topic Management:** Users can view topics, add questions, and list questions related to a specific topic.
- **Question & Answer Management:** Users can view a specific question, add answer options, and validate the correctness of an answer.
- **Quiz Taking:** Users can take quizzes on specific topics and get immediate feedback on their answers.
- **User Authentication:** Features for registering and logging in.
- **API Access:** Allows third-party integration to fetch random questions and validate answers.
- **Access Control:** Robust access control for different paths.
- **Styling:** Consistent styling throughout the application using a CSS framework accessed via CDN.

## Running the Application Locally

1. Clone the repository.
2. Ensure Docker and docker-compose are installed on your machine.
3. Navigate to the project root and run: ´docker-compose up´

4. Open your browser and navigate to `http://localhost:7777`.

**Admin Account Details:**
- Email: admin@admin.com
- Password: 123456

## Application Structure

- The code is located in the Code folder
- The project follows a three-tier architecture with views, controllers, services, and database.
- The Oak application is defined in `app.js` and exported.
- Dependencies are managed in `deps.js`.

## Access Control and Security

- Passwords are hashed using bcrypt and are not stored in plaintext.
- Only authorized users can access paths starting with `/topics` or `/quiz`.
- Root, `/auth`, and `/api` paths are accessible to all users.

## Acknowledgments

This project is developed as the final project in the cource CS-C3170 - Web Software Development at Aalto University in 2023. The responsible teacher for the course was Arto Hellas.

## Licence
This project is licensed under the terms of the MIT license. It can be found in the file LICENSE.
